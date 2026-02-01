# 実装開始

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
API実装の開始準備を行う。

## 入力
- `{{API_SPEC_DIR}}/openapi.yml`
- `{{API_SPEC_DIR}}/detail/`

## 指示
1. API仕様書を確認
2. 実装環境をセットアップ
3. プロジェクト構造を作成
4. 依存関係をインストール

## 成果物
- `{{IMPL_DIR}}/` の初期構造
- 実装計画（エンドポイント実装順序）

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "07-impl-start"
  status: "complete"
  comment: "実装準備完了"
  timestamp: 現在時刻を取得して記録
```
