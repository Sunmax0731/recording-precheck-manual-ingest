# Strict Manual Test Addendum

Codex 側では手動テスト未実施です。

## 作業ディレクトリ

`D:\AI\WindowsApp\recording-precheck-manual-ingest`

## 必要ファイル

- `samples/representative-suite.json`
- `src/product-profile/profile.json`
- `ui/`
- `docs/manual-test.md`
- `dist/recording-precheck-manual-ingest-docs.zip`

## セットアップ手順

1. 作業ディレクトリ `D:\AI\WindowsApp\recording-precheck-manual-ingest` で `npm test` を実行します。
2. `node src/cli/index.js samples/representative-suite.json` を実行します。
3. `ui/index.html` をブラウザで開き、代表シナリオの分類を確認します。

## ローカルサーバーやホストアプリ起動手順

ローカルサーバーは不要。必要に応じて `ui/index.html` をブラウザで開く。

## 実施手順

1. `npm test` を再実行する。
2. 実データ1件を `samples/representative-suite.json` と同じ形式で作成する。
3. CLIで検証する。
4. ホストUIまたは補助UIで表示する。
5. warning と fail の理由がユーザーに説明可能か確認する。

## 期待結果

- 自動テストが通る。
- docs ZIP が存在する。
- 実ホストまたは補助UIで最低1件の結果を確認できる。
- 未確認項目が release notes と一致する。

## 未実施の手動確認項目

- 実ホストUI表示
- 実素材/実ページ/実ファイルでの検査
- 配布導線のユーザー環境確認
- ストア/BOOTH向けスクリーンショット確認

