# API検証

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
API設計の整合性と完全性を検証する。

## 入力
- `{{API_SPEC_DIR}}/openapi.yml`
- `{{API_SPEC_DIR}}/endpoints/`

## 検証項目
1. **スキーマ整合性**: 参照が正しく解決されるか
2. **エンドポイント整合性**: パスパラメータが正しいか
3. **レスポンス整合性**: 成功/エラーレスポンスが定義されているか
4. **認証整合性**: セキュリティスキームが適用されているか
5. **例の整合性**: サンプルデータがスキーマに準拠しているか

## 成果物
- `{{API_SPEC_DIR}}/verify-report.md` - 検証レポート

## 指示
1. OpenAPI仕様をバリデーション
2. 不整合を検出・報告
3. 検証結果を出力

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "02-api-verify"
  status: "complete"
  comment: "検証結果を1行で"
  timestamp: 現在時刻を取得して記録
```
