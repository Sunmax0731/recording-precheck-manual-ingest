# 録画前チェック・手順書・録画素材取り込み

recording-precheck-manual-ingest は 動画制作者、チュートリアル収録者、配信準備担当者 向けの closed alpha プロダクトです。録画前の素材、手順、音声、画面サイズ、取り込み先を確認して失敗を減らす。

## Source

- PICKUP Rank: 46
- Domain / Idea No: WindowsApp / 5
- Repository: recording-precheck-manual-ingest
- 主な公開先: GitHub Release / BOOTH
- created_idea: `D:/AI/WindowsApp/created_idea_005_recording-precheck-manual-ingest`
- 同梱ZIP: `D:/AI/WindowsApp/created_idea_005_recording-precheck-manual-ingest/idea_005_recording-precheck-manual-ingest.zip`
- 開始時 README: 存在しない


## Alpha Scope

- 代表シナリオ4件の自動検証
- 必須項目不足、警告、混在バッチの分類
- ui/ のホスト連携シェル
- QCDS、security/privacy、traceability、release checklist、manual test docs
- docs ZIP: `dist/recording-precheck-manual-ingest-docs.zip`

## Commands

```powershell
npm test
node src/cli/index.js samples/representative-suite.json
npm run build:docs
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` にあります。

