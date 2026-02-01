# 実装

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
API仕様に基づいてエンドポイントを実装する。

## 入力
- `{{API_SPEC_DIR}}/openapi.yml`
- `{{API_SPEC_DIR}}/detail/`

## 成果物
- `{{IMPL_DIR}}/` - APIエンドポイント実装

## 指示
1. ルーティングを実装
2. リクエストバリデーションを実装
3. ビジネスロジックを実装
4. レスポンス生成を実装
5. エラーハンドリングを実装

## 注意事項
- 仕様書に記載のない機能を追加しない
- 仕様と実装の乖離を発見した場合は `STOP: SPEC ISSUE FOUND` を報告

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "08-impl-execute"
  status: "complete"
  comment: "実装内容を1行で"
  timestamp: 現在時刻を取得して記録
```
