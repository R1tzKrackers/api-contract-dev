# API修正

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
検証で発見された問題を修正する。

## 入力
- `{{API_SPEC_DIR}}/verify-report.md` - 検証レポート
- レビューフィードバック

## 成果物
- `{{API_SPEC_DIR}}/openapi.yml` の修正
- `{{API_SPEC_DIR}}/endpoints/` の修正

## 指示
1. 検証レポートの問題点を確認
2. 各問題に対する修正を実施
3. 修正内容を記録

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "03-api-fix"
  status: "complete"
  comment: "修正内容を1行で"
  timestamp: 現在時刻を取得して記録
```
