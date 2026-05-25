# VLDB 2027 No-API CPU Artifacts

This repository hosts cleaned release assets for eight CPU-only, no-API VLDB/PVLDB 2027 research artifacts.

The release tarballs exclude local manuscript TeX/PDF/build outputs, credentials, provider/live-model files, raw stores, indexes, caches, and files matched by the release secret-pattern scanner.

For each release asset, verify:

1. Anonymous download works without login.
2. SHA-256 matches the release manifest in the corresponding project packet.
3. The unpacked package passes `python scripts/no_api_cpu_audit.py --root . --json`.

Current public release: https://github.com/Haoyi-Zhang/vldb-2027-noapi-cpu-artifacts/releases/tag/vldb-2027-noapi-cpu-artifacts-v1

| Asset | Size | SHA-256 |
|---|---:|---|
| `cegar-sql-minimal-release-staging.tar.gz` | 4932704 | `ccc338fb438eaf8a3d84c2b4004a11a713ecf299c625daebcf5e46a09c6a3969` |
| `locallakeagent-minimal-release-staging.tar.gz` | 20703222 | `28783c428948ae1ff15d180e675d220a3c8152d77775b2dbbb53135b081f95a2` |
| `realops-sql-minimal-release-staging.tar.gz` | 14353956 | `3f3a0bb3af0300fcff949a0fa817f94e2675963e9e4606685ec2e7578dd9f219` |
| `semantic-query-budgets-minimal-release-staging.tar.gz` | 37099299 | `abf2422d7c8940fa6e41f08e46e5b59595137d79db3f830d4003c87b5e2c0c93` |
| `tablecompass-minimal-release-staging.tar.gz` | 41411344 | `aed9629668d56bbdaf5c6892a37163eba0e7afc2907693d60daddb42489df905` |
| `targetrecall-fvs-minimal-release-staging.tar.gz` | 7790402 | `ad6313f95224394aaf5a8caeb63cfebcfbe47ddfd1bbc549f7222935564ff313` |
| `udfwise-minimal-release-staging.tar.gz` | 24183342 | `b3c92eafa3e23c7102ca7f94fa11f0d4d02b634285c3e277148c82defbbc4141` |
| `vectoropsbench-minimal-release-staging.tar.gz` | 17633435 | `4e6cfa52cfed12cbca831e2b610d167e79577b91fbc68a3985da813ec2ac0082` |

The artifacts are intended for reviewer reproduction and audit of frozen CPU-only evidence packages. The May 25, 2026 refresh keeps p04/p05 live-provider modules out of the release while adding offline import stubs so reviewer audit commands execute in clean unpacked packages.
