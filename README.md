# moredaydevs-site

More Day Devs の公式サイト（https://www.moredaydevs.com/）の配信元です。
GitHub Pages で静的配信しています。

## 構成

| パス | 内容 | 正本 |
| --- | --- | --- |
| `index.html` | トップページ | `sudoku` リポジトリの `docs/official_site/index.html` |
| `assets/` | アプリアイコン、Google Play バッジ、アプリ画面 | 同上（`apps/sudoku_app/` 配下の既存アセット） |
| `sudoku/jp/privacy/` | プライバシーポリシー（日本語） | `apps/sudoku_app/store/privacy_policy_ja.html` |
| `sudoku/jp/terms/` | 利用規約（日本語） | `apps/sudoku_app/store/terms_of_service_ja.html` |
| `sudoku/en/privacy/` | プライバシーポリシー（英語） | `apps/sudoku_app/store/privacy_policy_en.html` |
| `sudoku/en/terms/` | 利用規約（英語） | `apps/sudoku_app/store/terms_of_service_en.html` |

法務ページの URL はアプリ内とストア掲載情報から参照されています。**パスを変えないこと。**

## 更新のしかた

このリポジトリを直接編集せず、`sudoku` リポジトリ側の正本を直してからここへ反映します。
アプリに同梱する版と公開版が食い違うのを防ぐためです。

`.nojekyll` は Jekyll の処理を止めるために置いています。消さないでください。

## 経緯

以前は Google Sites でホスティングしていましたが、ページ全体を 1 つの埋め込みブロックに
していたため、公開ページが真っ白になり、テキストが iframe に閉じて検索エンジンから
読まれず、モバイルで崩れていました（`sudoku` リポジトリの Issue #912）。
Google Sites のネイティブブロックでは元のレイアウトを再現できなかったため、
静的配信へ移しました。
