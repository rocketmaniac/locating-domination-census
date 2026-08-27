# Deposited objects (orders 10–26)

This file is for readers who need checksums. The mathematical claims
are in the [README](README.md) and the
[preprint](https://github.com/rocketmaniac/ld-strict-bound-v2-artifacts/releases/download/v2/ld-strict-bound-v2-preprint.pdf).

Release [v2](https://github.com/rocketmaniac/ld-strict-bound-v2-artifacts/releases/tag/v2)
holds the 10–26 evidence archive and the paper-cited reports. The git
tree holds the small JSON files and `SHA256SUMS`. The archive itself
is release-only (299,594,503 bytes). Order-28 certificates are not
part of this deposit.

## SHA-256 identities cited by the paper

| Object | SHA-256 |
| --- | --- |
| `verification-v2/report.json` (file) | `cb9b471a15add06ccaa1d65da0a0a049cba5be197bb9b33a9ad8b456f80c942c` |
| report payload | `46a6bad91d3d2636c6e757125be93534a28ea404df15bc98c85ea0b845803512` |
| input manifest file | `a4b067bc3965c16e7a574039942ea60a4d22321431dace2d440bd00cda6b1641` |
| archive v3 object | `7dae0e0c977f1c266466884153657ec363973b29c152dfc805ed8724e91335ee` (299,594,503 bytes) |

The verification report records `expected=193969`, `verified=193969`,
`status_counts.non_tight=193969`, `status_counts.tight=0`,
`proof_count=0`. Remaining manuscript hashes are in the preprint
section *Frozen identities*.

Every file in the git tree (and the release archive) is listed in
`SHA256SUMS`.

## Release assets

- `ld-strict-bound-v2-preprint.pdf` — preprint
- `locating-domination-orders10-26-v2.tar.zst.part-000` — archive
- `SHA256SUMS`, `report.json`, input manifest, and the small
  campaign/archive JSON files

## Byte-identity check

```console
shasum -a 256 -c SHA256SUMS
python3 -c "import json; r=json.load(open('verification-v2/report.json')); assert r['expected']==r['verified']==193969; assert r['status_counts']=={'non_tight':193969,'tight':0}; assert r['proof_count']==0"
```
