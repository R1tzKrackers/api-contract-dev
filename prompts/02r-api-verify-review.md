# API検証レビュー

## 目的
API検証結果の人間レビューを実施する。

## レビュー対象
- `{{API_SPEC_DIR}}/verify-report.md`

## 判定基準
- 重大な不整合がないこと
- 全てのエンドポイントが検証済みであること

## 判定
- **承認**: 次フェーズ（詳細設計）へ進む
- **差し戻し**: API修正フェーズに戻る
- **再設計**: API設計フェーズに戻る

## 指示
検証結果を確認し、次のアクションを決定せよ。

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "02r-api-verify-review"
  status: "complete"  # または "reject"（差し戻しの場合）
  comment: "レビュー結果を1行で"
  target: "03-api-fix"  # 差し戻し先（rejectの場合のみ）
  timestamp: 現在時刻を取得して記録
```
