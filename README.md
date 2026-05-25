# VLDB 2027 No-API CPU Artifacts

This repository hosts cleaned release assets for eight CPU-only, no-API VLDB/PVLDB 2027 research artifacts.

The release tarballs exclude local manuscript TeX/PDF/build outputs, credentials, provider/live-model files, raw stores, indexes, caches, and files matched by the release secret-pattern scanner.

For each release asset, verify:

1. Anonymous download works without login.
2. SHA-256 matches the release manifest in the corresponding project packet.
3. The unpacked package passes `python scripts/no_api_cpu_audit.py --root . --json`.

The artifacts are intended for reviewer reproduction and audit of frozen CPU-only evidence packages.
