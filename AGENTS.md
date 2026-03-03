<INSTRUCTIONS>
# Global agent instructions (for this repository)

- 日本語で回答すること。
- 無駄な共感や感嘆符は使わないこと。
- ビジネス用途に適した専門用語を用いること。
- 分からないことは推測で断定せず、「分かりません」と明示すること。
- 技術内容については、可能な範囲で根拠（バージョン・前提条件など）を示すこと。

---

# Repository purpose / working agreement

本リポジトリは、ae-framework の **input-only spec repo**（入力のみリポジトリ）です。  
ここでは **仕様と前提の管理**のみを行い、実装・テスト・機械可読なAPI契約・CI・中間生成物は **出力（別リポジトリ/別工程）**として扱います。

方針のSSOT（一次情報）:
- `itdojp/ae-framework` の `docs/product/INPUT-ONLY-SPEC-REPO-PATTERN.md`

## 入力（このリポジトリに存在してよいもの）
- 仕様（人間可読）: `spec/*`
- 上級工程の前提/制約: `assumptions.md`
- 実装タスク（出力定義）: `task.md`

## 禁止（このリポジトリに置かない）
ディレクトリ名に依らず、次は **出力（生成物）**として扱い、コミットしません。

- 実装コード（例: `src/`, `apps/`, `packages/`）
- テスト（例: `tests/`）
- 機械可読な API 契約（OpenAPI / JSON Schema / `.proto` / GraphQL SDL / AsyncAPI 等）
- 生成物を前提にする CI（例: `.github/workflows/*`）
- 中間生成物・レポート（例: `artifacts/**`, `.ae/**`, `reports/**`）

## 本リポジトリでやること（エージェントの責務）
- 仕様の曖昧さ/矛盾の解消（`spec/` の改訂）
- 出力に必要な前提条件の明文化（`assumptions.md` の更新）
- 生成すべき成果物の定義更新（`task.md` の更新）

## 仕様変更PRの完了条件（DoD）
- 変更が `spec/` / `assumptions.md` / `task.md` の範囲に限定されている
- 「入力のみ」方針（禁止物の非混入）を満たす

</INSTRUCTIONS>
