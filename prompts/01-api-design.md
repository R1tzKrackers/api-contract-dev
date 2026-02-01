# API設計

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
APIのスキーマとエンドポイントを設計する。

## 入力
- プロジェクト要件
- 既存システムとの連携要件（あれば）

## 成果物
- `{{API_SPEC_DIR}}/openapi.yml` - OpenAPI仕様書
- `{{API_SPEC_DIR}}/endpoints/` - エンドポイント定義

## 指示
1. API全体のスコープを定義
2. リソースとエンドポイントを洗い出し
3. OpenAPI形式で仕様を記述
4. リクエスト/レスポンススキーマを定義
5. エラーレスポンスを定義

## 出力形式
```yaml
# {{API_SPEC_DIR}}/openapi.yml
openapi: 3.0.0
info:
  title: {{PROJECT_NAME}} API
  version: 1.0.0
paths:
  /resource:
    get:
      summary: リソース一覧取得
      responses:
        '200':
          description: 成功
```

## 注意事項
- RESTful設計原則に従う
- 命名規則を統一する
- バージョニング戦略を明記する

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "01-api-design"
  status: "complete"
  comment: "設計内容を1行で"
  timestamp: 現在時刻を取得して記録
```
