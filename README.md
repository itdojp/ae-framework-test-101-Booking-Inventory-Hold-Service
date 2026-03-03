# Booking / Inventory Hold Service — Input Spec Repo

本リポジトリは、ae-framework の **input-only spec repo** パターンに基づくテスト入力です。
ここには **仕様（人間可読）と上級工程で固定した前提**のみを保持し、実装・テスト・機械可読なAPI契約・CI・中間生成物は **出力（別リポジトリ/別工程）**として生成します。

方針のSSOT（一次情報）:
- `itdojp/ae-framework` の `docs/product/INPUT-ONLY-SPEC-REPO-PATTERN.md`

## Inputs (this repo)

- 仕様: `spec/`
- 実装タスク（出力定義）: `task.md`
- 前提/制約（上級工程）: `assumptions.md`

## Outputs (generated elsewhere)

ディレクトリ名に依らず、次は **出力（生成物）**として扱い、本リポジトリにコミットしません。

- 実装コード（例: `src/`, `apps/`, `packages/`）
- テスト（例: `tests/`）
- 機械可読な API 契約（OpenAPI / JSON Schema / `.proto` / GraphQL SDL / AsyncAPI 等）
- 生成物を前提にする CI（例: `.github/workflows/*`）
- 中間生成物・レポート（例: `artifacts/**`, `.ae/**`, `reports/**`）

## Notes (harness responsibility)

- Input Gate（入力健全性）と Synthesis Gate（合成実行）は、ハーネス側（CIまたはローカルランナー）で実行する。
- 再現性のため、使用した `ae-framework` のコミットSHAおよび実行環境（Node/pnpm等）は、出力側に記録する。
