# Paper and data license (CC BY 4.0)

This file licenses **paper, originally generated data, and released analysis
evidence**. It does **not** license source code. Source, scripts, tests, and
ops tooling are MIT; see `LICENSE` and `LICENSE-DECISION.md`.

Copyright (c) 2026 ROCKETMANIA INC

`AUTHORS-CREDIT.md.template` and `CITATION.cff.template` still contain
`REPLACE` placeholders for individual author, ORCID, and affiliation
credits. Those personal credits are separate from this copyright holder.

## What this license covers

When material in the following classes is **intentionally released** (public
repository files, a deposit, or a publication package), it is offered under
Creative Commons Attribution 4.0 International (CC BY 4.0):

- the manuscript and paper-facing text under `publication/paper/` and
  related publication prose (`publication/literature-dossier.md`,
  `publication/references.bib`, and other `publication/` documents that are
  not third-party);
- originally generated graphs, tables, summaries, certificates, and other
  scientific outputs that this project created;
- curated fixtures that are **this project's** generated records (not
  third-party excerpts).

The SPDX identifier is `CC-BY-4.0`. The legal code is
<https://creativecommons.org/licenses/by/4.0/legalcode>. A human-readable
deed is <https://creativecommons.org/licenses/by/4.0/>.

You are free to share and adapt that released material, including
commercially, provided you give appropriate credit, provide a link to the
license, and indicate if changes were made. No additional restrictions may
be applied that legally restrict others from doing anything the license
permits. The license does not grant patent, trademark, or publicity rights,
and it offers the material as-is without warranty.

## What this license does not grant

**Code.** `src/`, `scripts/`, `tests/`, `ops/` tooling, GitHub workflow
sources, and the installable `graph-discovery-lab` package remain MIT.

**Local-only analysis evidence.** Trees such as `analysis/` and `results/`
are operational or write-once evidence roots. Many paths are gitignored,
machine-local, or not a public archive. This file does **not** claim that
those trees are published, complete, or redistributable merely because they
exist on a workstation. If and when a named evidence bundle is later
included in a reviewed public release or deposit, the **intent** is that
*this project's originally generated contents of that bundle* are CC BY 4.0,
subject to the third-party exclusions below.

**Third-party material (unchanged licenses).** This grant does not relicense:

- nauty / Traces and related binaries or sources;
- CaDiCaL;
- drat-trim and other independent proof checkers;
- Holt and Royle vertex-transitive census archives and the verbatim
  `data/fixtures/alltrans26_k=03.g6` excerpts (already CC BY 4.0 from their
  authors; attribution and DOI still required — see
  `docs/research-notes.md`);
- Brinkmann and Van Overberghe 2026 material under
  `external/brinkmann-van-overberghe-2026/` (arXiv
  nonexclusive-distrib-1.0 and House of Graphs terms as recorded there);
- Python and system dependencies, which keep their own licenses.

Copied third-party excerpts remain under their upstream terms even when
stored next to originally generated files.

## How to give credit

Until citation metadata is finalized, credit the repository
<https://github.com/rocketmaniac/cubic-bipartite-domination> and this
copyright line. After `CITATION.cff` exists, use that reviewed citation.
For Holt–Royle fixtures or any redistributed derived census data, also
retain their required attribution and DOI.
