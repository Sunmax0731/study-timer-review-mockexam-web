# study-timer-review-mockexam-web

学習タイマー・復習・模試Web は、学習タイマー、復習キュー、模試フローを静的Webでまとめるです。

## Closed Alpha Scope

- Rank: 35
- Tier / Score: P1 / 60
- Domain / Idea No: WebApp / 2
- 主な公開先: GitHub Pages / GitHub Release
- GitHub: https://github.com/Sunmax0731/study-timer-review-mockexam-web
- Prerelease: https://github.com/Sunmax0731/study-timer-review-mockexam-web/releases/tag/v0.1.0-alpha.1

## 実装概要

- `src/core`: 製品プロファイルと代表シナリオ評価
- `src/validators`: 期待結果検証
- `src/report`: 検証レポート生成
- `src/review-model`: レビューゲートと責務モデル
- `src/cli`: `samples/representative-suite.json` の自動検証

## 代表データ

`samples/representative-suite.json` は `happy-path`、`missing-required`、`warning`、`mixed-batch` を含みます。

## 検証

```powershell
cd D:\AI\WebApp\study-timer-review-mockexam-web
cmd.exe /d /s /c npm test
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` を参照してください。
