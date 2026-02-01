# 詳細設計

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
エンドポイントの詳細仕様とデータモデルを設計する。

## 入力
- `{{API_SPEC_DIR}}/openapi.yml`

## 成果物
- `{{API_SPEC_DIR}}/detail/models.yml` - データモデル詳細
- `{{API_SPEC_DIR}}/detail/handlers.yml` - ハンドラ仕様
- `{{API_SPEC_DIR}}/detail/validation.yml` - バリデーションルール

## 指示
1. 各エンドポイントの処理フローを定義
2. データモデルの詳細（バリデーション、制約）を定義
3. エラーハンドリング方針を定義
4. ページネーション、フィルタリング仕様を定義

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "04-detail-design"
  status: "complete"
  comment: "設計内容を1行で"
  timestamp: 現在時刻を取得して記録
```
