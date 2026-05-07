# インストールガイド

## Closed Alpha Package

1. GitHub Release `v0.1.0-alpha.1` から assets を取得する。
2. `dist/recording-precheck-manual-ingest-docs.zip` を展開して README と manual-test を確認する。
3. repo を clone する場合:

```powershell
git clone https://github.com/Sunmax0731/recording-precheck-manual-ingest.git
cd recording-precheck-manual-ingest
npm test
```

## Host Setup

1. 作業ディレクトリ `D:\AI\WindowsApp\recording-precheck-manual-ingest` で `npm test` を実行します。
2. `node src/cli/index.js samples/representative-suite.json` を実行します。
3. `ui/index.html` をブラウザで開き、代表シナリオの分類を確認します。

