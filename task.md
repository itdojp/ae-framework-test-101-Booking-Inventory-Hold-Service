# Task (Benchmark) — Booking / Inventory Hold Service

本リポジトリは input-only spec repo です。  
この `task.md` は、別リポジトリ/別工程（出力側）で生成・実装すべき内容を定義します。

## Inputs (this repo)

- `spec/`
- `assumptions.md`

## Outputs (generated elsewhere)

### 1) 実装（必須）

- `spec/` の仕様に基づく Booking / Inventory Hold Service の実装

### 2) 機械可読な API 契約（必須）

ディレクトリ名に依らず、機械可読な API 契約（例: OpenAPI）を出力すること。

### 3) テスト/CI（任意）

- build/test/lint を実行できる最小のテストおよびCIを整備してよい（出力扱い）

## Acceptance Criteria (minimum)

- Hold/Confirm/Cancel/Expire を含む基本ユースケースが成立する
- 二重確保（過剰引当/二重予約）が発生しない（少なくとも単体・同時実行の基本ケース）
