# Locating-domination strict-bound v2 artifacts

Public evidence deposit for the preprint *A Certificate-Backed
Locating-Domination Strict-Bound Census for Connected Cubic Bipartite
Graphs of Orders 10–26*.

**Author / copyright.** ROCKETMANIA INC.  
**License.** Originally generated contents are [CC BY 4.0](LICENSE-DATA.md).  
**Claim (only public claim).** Twin-free connected simple cubic bipartite
graphs of even order 10–26: **193,969** graphs, **193,969** non-tight,
**0** tight. Independently verified. Exact \(\gamma_L\) is withheld.
Order 28 is withheld.

This repository is an artifacts-only deposit. It is not the research
source tree.

## Frozen identities (paper-cited)

| Object | SHA-256 |
| --- | --- |
| `verification-v2/report.json` (file) | `cb9b471a15add06ccaa1d65da0a0a049cba5be197bb9b33a9ad8b456f80c942c` |
| report payload | `46a6bad91d3d2636c6e757125be93534a28ea404df15bc98c85ea0b845803512` |
| input manifest file | `a4b067bc3965c16e7a574039942ea60a4d22321431dace2d440bd00cda6b1641` |
| archive v3 object | `7dae0e0c977f1c266466884153657ec363973b29c152dfc805ed8724e91335ee` (299,594,503 bytes) |

Report fields: `expected=193969`, `verified=193969`,
`status_counts.non_tight=193969`, `status_counts.tight=0`,
`proof_count=0`. Remaining manuscript hashes are in the preprint frozen
identities section.

## Release assets

The 299,594,503-byte archive and the paper-cited reports/manifests are
attached to GitHub Release **v2**:

https://github.com/rocketmaniac/ld-strict-bound-v2-artifacts/releases/tag/v2

- `locating-domination-orders10-26-v2.tar.zst.part-000` — archive v3 object
- `SHA256SUMS` — SHA-256 of every file deposited here (including the archive)
- `report.json` — independent verification report
- manifests: input manifest, campaign provenance/config/summaries, archive index and provenance

The git tree holds the small paper-cited JSON files and `SHA256SUMS`.
The archive is release-only (286 MiB; under the 2 GiB GitHub asset limit).

## How to check

```console
shasum -a 256 -c SHA256SUMS
python3 -c "import json; r=json.load(open('verification-v2/report.json')); assert r['expected']==r['verified']==193969; assert r['status_counts']=={'non_tight':193969,'tight':0}; assert r['proof_count']==0"
```
