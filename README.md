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
| `cegar-sql-minimal-release-staging.tar.gz` | 4932929 | `0334d83904a48859ca1ecd8973e8574106d33dcd7df1adbcb59ee08a44c8225b` |
| `locallakeagent-minimal-release-staging.tar.gz` | 20702780 | `b73fbb57e2a1c0d272819fae5ff216704c270c504fefc0068159c21ec4b5634b` |
| `realops-sql-minimal-release-staging.tar.gz` | 14354196 | `3b6d09497f2eba52572f5a067f7288cc73eee3dd89acc9efeee1171095ddebc2` |
| `semantic-query-budgets-minimal-release-staging.tar.gz` | 37100028 | `fea8eee08b39bc0efd0561a93ae7107e7d14c421a96b48a9de6de82d33224e20` |
| `tablecompass-minimal-release-staging.tar.gz` | 41411219 | `e9284448019896859f15c114c637d9d03085ec95a0c34860da04697189d8bd79` |
| `targetrecall-fvs-minimal-release-staging.tar.gz` | 7790136 | `6a6503de6aaeff90dab442e07170435e08a4946791a82ff47aac4798183c1c47` |
| `udfwise-minimal-release-staging.tar.gz` | 24183409 | `41e5049187ea7b5b59f69885b996e1b359b4671240f6a042e49cfc64190d4155` |
| `vectoropsbench-minimal-release-staging.tar.gz` | 17633604 | `12de13dc918af163f553af62da298eca4bac19f9be805ffae042fd044b4f777c` |

The artifacts are intended for reviewer reproduction and audit of frozen CPU-only evidence packages. The May 25, 2026 refresh keeps p04/p05 live-provider modules out of the release while adding offline import stubs so reviewer audit commands execute in clean unpacked packages.
