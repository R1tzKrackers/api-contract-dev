# 実装検証

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
実装がAPI仕様に準拠しているか検証する。

## 入力
- `{{API_SPEC_DIR}}/openapi.yml`
- `{{IMPL_DIR}}/`
- `{{TEST_DIR}}/`

## 検証項目
1. 全エンドポイントが実装されているか
2. リクエスト/レスポンスが仕様通りか
3. テストがパスしているか
4. カバレッジが十分か

## 成果物
- 検証レポート

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "10-impl-verify"
  status: "complete"
  comment: "検証結果を1行で"
  timestamp: 現在時刻を取得して記録
```
