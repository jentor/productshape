---
'@prodshape/integration-openspec': patch
'@prodshape/cli': patch
---

`prodshape integration add|update|remove openspec` no longer rewrites your `openspec/config.yaml`. Hand-written `context: |` blocks are no longer folded into 80-column `>-` blocks with blank lines between every line, and comments, key order and untouched entries are kept byte-for-byte. Only the PDaC-managed parts of the file change.
