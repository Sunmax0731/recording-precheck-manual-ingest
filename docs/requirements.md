# 要件定義

## 目的

録画前チェック・手順書・録画素材取り込み は、動画制作者、チュートリアル収録者、配信準備担当者 が 録画前の素材、手順、音声、画面サイズ、取り込み先を確認して失敗を減らす。

## Source

- PICKUP Rank: 46
- Domain / Idea No: WindowsApp / 5
- Repository: recording-precheck-manual-ingest
- created_idea: `D:/AI/WindowsApp/created_idea_005_recording-precheck-manual-ingest`
- ZIP: `D:/AI/WindowsApp/created_idea_005_recording-precheck-manual-ingest/idea_005_recording-precheck-manual-ingest.zip`
- README確認: 開始時点では正式 repo が存在しないため、README.md は存在しない。

## Functional Requirements

- R1: sessionName、captureSource、manualSteps、assetFolder を必須項目として検査する。
- R2: 必須項目不足は fail として分類する。
- R3: `audioUnchecked` が true の場合は warning として分類し、手動確認理由を返す。
- R4: 複数アイテムの mixed-batch を pass / warning / fail に集計する。
- R5: 結果を CLI と docs/release evidence で再利用できる形にする。

## Non Functional Requirements

- UTF-8 で Markdown / JSON / JS / HTML / Python を保存する。
- 外部通信を既定で行わず、サンプルとローカル入力だけで検証できる。
- 手動テスト未実施であることを release 前 docs に明記する。

