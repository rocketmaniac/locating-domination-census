# Locating-domination on twin-free cubic bipartite graphs

Read the preprint first:

**[A Certificate-Backed Locating-Domination Census for Twin-Free Connected Cubic Bipartite Graphs of Orders 10–28](https://github.com/rocketmaniac/ld-strict-bound-v2-artifacts/releases/download/v2/ld-strict-bound-v2-preprint.pdf)**  
(Paul A. Barros, 26 August 2026).

A locating-dominating set is a dominating set that also separates the
vertices outside it. Write $\gamma_L(G)$ for the locating-domination
number. On twin-free graphs one can ask, in the spirit of Slater,
whether $\gamma_L = n/2$ is attained. This note studies that question
on the twin-free connected cubic bipartite graphs of even order.

## Finite statements

These are census statements, not an arbitrary-order theorem.

- **Orders 10–26.** There are 193,969 such graphs. Each has a
  locating-dominating set of size at most $n/2-1$: all are
  *non-tight*, and none is *tight*. The classification was
  independently rechecked.
- **Order 28.** There are 1,650,044 such graphs. The exact
  $\gamma_L$ histogram, independently rechecked, is
  1,619,934 / 30,067 / 43 at the values 10 / 11 / 12
  (hence $\gamma_L \le 12 \le n/2-1$). The table is in the PDF.

Exact $\gamma_L$ values for the individual order-10–26 graphs are
not published here. **Order 30 is not claimed.**

## Ordinary domination is a different census

This work is about $\gamma_L$, not ordinary domination $\gamma$ or
independent domination $i(G)$. Brinkmann and Van Overberghe already
computed $\gamma$ and $i(G)$ on cubic graphs through order 26
([arXiv:2606.16698](https://arxiv.org/abs/2606.16698)); Van Overberghe
has since carried that $\gamma$ / $i(G)$ census through order 36.

## What is *not* on GitHub

The order-28 certificates (about 21 GiB) are not uploaded. This
repository is a small public deposit, not the research source tree.
Originally generated contents are [CC BY 4.0](LICENSE-DATA.md).

Release [v2](https://github.com/rocketmaniac/ld-strict-bound-v2-artifacts/releases/tag/v2)
holds the preprint PDF and the 10–26 evidence archive (about 286 MiB).

## How to check a small example

The subsection *Certificate validation* in the PDF says how a single
graph is checked: reconstruct the stored locating-dominating set and
verify domination and the distinct $N(v)\cap D$ signatures directly
on the graph. File hashes for the deposited 10–26 objects are in
[`ARTIFACTS.md`](ARTIFACTS.md).
