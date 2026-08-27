# Locating-domination on twin-free cubic bipartite graphs

Read the preprint first:

**[A Certificate-Backed Locating-Domination Census for Twin-Free Connected Cubic Bipartite Graphs of Orders 10–28](https://github.com/rocketmaniac/locating-domination-census/releases/download/v2/locating-domination-census.pdf)**  
(Paul A. Barros, 27 August 2026).

A locating-dominating set, in the sense of Slater, is a dominating set
that also separates the vertices outside it. Write $\gamma_L(G)$ for
the locating-domination number. This is distinct from ordinary
domination $\gamma(G)$ and independent domination $i(G)$.

On twin-free graphs one already has $\gamma_L\le n/2$. This note asks
whether that bound is attained on the twin-free connected cubic
bipartite graphs of even order 10 through 28.

## Finite statements

These are census statements, not an arbitrary-order theorem.

- **Orders 10–26.** There are 193,969 such graphs. Each has a
  locating-dominating set of size at most $n/2-1$, so none attains
  $\gamma_L=n/2$. The classification was independently rechecked.
- **Order 28.** There are 1,650,044 such graphs. The exact
  $\gamma_L$ histogram, independently rechecked, is
  1,619,934 / 30,067 / 43 at the values 10 / 11 / 12
  (hence $\gamma_L\le 12\le n/2-1$). The table is in the PDF.

Exact $\gamma_L$ values for the individual order-10–26 graphs are
not published here. **Order 30 is not claimed.**

## Ordinary domination is a different census

This work is about $\gamma_L$, not ordinary domination $\gamma$ or
independent domination $i(G)$. Brinkmann and Van Overberghe already
computed $\gamma$ and $i(G)$ on cubic graphs through order 26
([arXiv:2606.16698](https://arxiv.org/abs/2606.16698)).

## What is *not* on GitHub

The order-28 certificates (about 21 GiB) are not uploaded. This
repository is a small public deposit, not the research source tree.
Originally generated contents are [CC BY 4.0](LICENSE-DATA.md).

Release [v2](https://github.com/rocketmaniac/locating-domination-census/releases/tag/v2)
holds the preprint PDF and the 10–26 evidence archive (about 286 MiB).

## How to check a small example

The subsection *Certificate validation* in the PDF says how a single
graph is checked: reconstruct the stored locating-dominating set and
verify domination and the distinct sets $N(v)\cap D$ directly
on the graph. File hashes for the deposited 10–26 objects are in
[`ARTIFACTS.md`](ARTIFACTS.md) and `SHA256SUMS`, not in the paper.
