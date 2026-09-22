<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [topological spectrum](../../../../../../spectrum-topology.md) can be described sequentially by [based spaces](../../../../../../based-space.md) $E_j$, $j\ge0$, and structure maps

$$
\sigma_j:S^1\wedge E_j\longrightarrow E_{j+1}.
$$

Iterating these maps gives compatible maps $S^{k-j}\wedge E_j\to E_k$. Equivalently, an [indexed prespectrum](../../../../../../indexed-prespectrum.md) on a [universe for spectra](../../../../../../universe-for-spectra.md) $U$ has spaces $E(V)$ and unital associative structure maps $S^{W\ominus V}\wedge E(V)\to E(W)$ for finite-dimensional inclusions $V\subset W\subset U$. Here $S^A$ denotes the [one-point compactification](../../../../../../alexandroff-extension.md) of the real [inner product space](../../../../../../inner-product-space.md) $A$.

A [map of topological spectra](../../../../../../map-of-topological-spectra.md) $u:D\to E$ is a family of based maps $u_j:D_j\to E_j$ satisfying

$$
u_{j+1}\sigma_j^D=\sigma_j^E(1\wedge u_j).
$$

The indexed version requires the same compatibility for every inclusion of indexing subspaces. These are point-set maps, before passing to [spectrum homotopy](../../../../../../spectrum-homotopy.md) or the [stable homotopy category](../../../../../../stable-homotopy-category.md).

An [Omega-spectrum](../../../../../../omega-spectrum.md) is a [topological spectrum](../../../../../../spectrum-topology.md) whose adjoint structure maps

$$
E_j\longrightarrow\Omega E_{j+1}
$$

are [weak homotopy equivalences](../../../../../../weak-homotopy-equivalence.md). Consequently $\pi_kE=\pi_{k+j}E_j$ whenever $k+j\ge0$, using the structure identifications. In the genuine indexed point-set convention, the word spectrum already includes the stronger condition that $E(V)\to\Omega^{W\ominus V}E(W)$ is a homeomorphism; a general system without that condition is called an [indexed prespectrum](../../../../../../indexed-prespectrum.md). Its associated spectrum is obtained by [spectrification](../../../../../../spectrification.md). The sequential and indexed conventions present the same stable theory.

A [cell spectrum](../../../../../../cell-spectrum.md) is built from the zero [topological spectrum](../../../../../../spectrum-topology.md) by successive stable cell attachments. Concretely, attach a free spectrum on the inclusion $S^{m-1}\hookrightarrow D^m$ at some level $j$ by a pushout along its boundary map; its quotient is the stable cell sphere $\Sigma^{m-j}\mathbb S$. Iterating such attachments and taking the colimit gives a [cell spectrum](../../../../../../cell-spectrum.md), with successive quotients wedges of integer [suspensions of spectra](../../../../../../suspension-of-spectra.md) of the [sphere spectrum](../../../../../../sphere-spectrum.md). Negative cell degrees are allowed by choosing $j>m$. In the genuine indexed model apply [spectrification](../../../../../../spectrification.md) to this cellular prespectrum. **The compatibility of the structure maps is part of both the objects and their maps.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
