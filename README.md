# かいものメモ

家族用の買い物メモアプリです。リストは各スマホの中に保存されます（家族間では同期しません）。

## スマホで使う（2通り）
- **Web版**：Chromeで https://t-nakanishi729.github.io/kaimono-memo/ を開き、「⋮」→「ホーム画面に追加」
- **APK版**：「Releases」の最新版から kaimono-memo.apk をダウンロードしてインストール

## よく買うものを変える
docs/index.html の `QUICK=[...]` を書き換えて保存（Commit）すると、Web版はすぐ、APKは数分後に新しい版ができます。

## 仕組み
- docs/ … Web版（GitHub Pagesで公開）。APKも同じ画面を使います
- app/ … Androidアプリ本体
- .github/workflows/build-apk.yml … mainに変更が入るたびにAPKを自動ビルドしてReleasesに置きます
