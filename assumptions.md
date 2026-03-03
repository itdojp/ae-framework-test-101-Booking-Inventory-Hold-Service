# Assumptions / Constraints (Upstream Decisions)

本ファイルは、上級工程で固定した「前提条件」を記述します。  
これらは input-only spec repo における入力の一部ですが、実装・テスト・CI・契約等の生成物は本リポジトリに置きません。

## Target Stack (recommended)

- Language: TypeScript
- Runtime: Node.js `>=20.11 <23`
- Package manager: pnpm `10.x`

根拠:
- `itdojp/ae-framework` の `package.json`（`engines.node`, `packageManager`）

## Security / Assurance

- 本タスクは研究/検証用途であり、実運用レベルの安全性保証を目的としない。
