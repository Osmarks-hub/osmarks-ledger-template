# osmarks ledger

This repository is your osmarks ledger. It is the only copy that counts; osmarks keeps just a short-lived cache.

- One deal per file: `records/<year>/<record id>.json`
- Format: osmarks Record v0 (`schema_version: v0`). `direction`: `buy` or `sell` (sell = paid sales only); `price`: `{amount, currency, kind}`
- `confidence`: `self` (you), `peer` (other side confirmed), `receipt` (signed receipt), `imported`, `imported_sampled`
- Records are never edited: a correction is a new record whose `supersedes` lists the old ids
- `test: true` marks the install self-check; kept forever, hidden in pages and totals

Your assistant writes here through osmarks when you say you bought or sold something. You can read, edit or delete any file yourself.
Questions: support@osmarks.com
