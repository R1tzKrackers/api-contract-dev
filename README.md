# API Contract Framework

**API駆動開発フレームワーク / API-Driven Development Framework**

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)]()
[![Phase Manager](https://img.shields.io/badge/requires-Phase%20Manager-green.svg)]()

---

## 概要 / Overview

API Contract Frameworkは、API設計を起点とした開発ワークフローを提供するフレームワークです。
OpenAPIスキーマ設計から実装、テストまでの一貫したフローを定義します。

*API Contract Framework provides an API-first development workflow.
It defines a consistent flow from OpenAPI schema design to implementation and testing.*

---

## 特徴 / Features

- **API駆動設計** - OpenAPI仕様を起点とした開発フロー
  *API-Driven Design - Development flow starting from OpenAPI specification*

- **契約凍結** - API仕様凍結後の変更を防止
  *Contract Freeze - Prevents specification changes after API design completion*

- **テスト統合** - API仕様に基づくテスト自動生成支援
  *Test Integration - Supports test generation based on API specification*

---

## ワークフロー / Workflow

```
[Setup]
  00c-project-config    プロジェクト設定 / Project Configuration
       |
[Design - API]
  01-api-design         API設計 / API Design
  01r-api-review        API設計レビュー / API Design Review
  02-api-verify         API検証 / API Verification
  02r-api-verify-review API検証レビュー / API Verification Review
  03-api-fix            API修正（任意）/ API Fix (optional)
       |
[Design - Detail]
  04-detail-design      詳細設計 / Detail Design
  04r-detail-review     詳細設計レビュー / Detail Review
       |
[Handoff]
  05-handoff-check      引継ぎ判定 / Handoff Check
  06-design-freeze      契約凍結 / Contract Freeze
       |
[Implementation]
  07-impl-start         実装開始 / Implementation Start
  08-impl-execute       実装 / Implementation Execute
  09-test-execute       テスト実装 / Test Implementation
  10-impl-verify        実装検証 / Implementation Verification
  10r-impl-verify-review 実装検証レビュー / Implementation Review
  11-impl-complete      実装完了 / Implementation Complete
```

---

## ディレクトリ構成 / Directory Structure

```
api-contract-dev/
├── framework.yml      # フレームワークマニフェスト / Framework manifest
├── prompts/           # フェーズ別プロンプト / Phase-specific prompts
└── templates/         # テンプレート / Templates
    └── AGENTS.md.template
```

---

## 使用方法 / Usage

### 前提条件 / Prerequisites

- [Phase Manager](https://github.com/R1tzKrackers/phase-manager) がインストール済みであること

### セットアップ / Setup

1. Phase Managerの初期化フェーズで本フレームワークを選択
2. `project-config.yml` でプロジェクト固有の設定を行う

---

## 変数 / Variables

| 変数 / Variable | 説明 / Description |
|-----------------|---------------------|
| `{{PROJECT_NAME}}` | プロジェクト名 / Project name |
| `{{DESIGN_ROLE}}` | 設計担当ロール名 / Design role name |
| `{{IMPL_ROLE}}` | 実装担当ロール名 / Implementation role name |
| `{{API_SPEC_DIR}}` | API仕様書ディレクトリ / API spec directory |
| `{{IMPL_DIR}}` | 実装ディレクトリ / Implementation directory |
| `{{TEST_DIR}}` | テストディレクトリ / Test directory |

---

## ライセンス / License

MIT License

---

## 関連 / Related

- [Phase Manager](https://github.com/R1tzKrackers/phase-manager) - ワークフロー管理ツール
