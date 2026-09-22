<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [general algorithm in the SCI hierarchy](../../../../../../general-algorithm-in-the-sci-hierarchy.md) $\Gamma:\Omega\to\mathcal M$ reads a finite set $\Lambda_\Gamma(A)\subset\Lambda$ on each input $A$. Its output depends only on those values, and whenever another input $B$ has the same values on $\Lambda_\Gamma(A)$, the algorithm requests the same finite set and gives the same output. A [tower of algorithms](../../../../../../tower-of-algorithms.md) of height $k$ satisfies

$$
\Xi(A)=\lim_{n_k\to\infty}\cdots\lim_{n_1\to\infty}
\Gamma_{n_k,\ldots,n_1}(A)
$$

for every $A\in\Omega$. The [Solvability complexity index](../../../../../../solvability-complexity-index.md) is the least such $k$, with value zero when one finite algorithm computes $\Xi$ exactly.

We reduce a known height-three [finite-column decision problem](../../../../../../finite-column-decision-problem.md) to spectral computation. Let $(a_{ij})_{i,j\in\mathbb Z}$ be a bi-infinite zero-one matrix and let $\Xi_{\rm col}$ ask whether there is a number $D$ such that every column either contains fewer than $D$ ones or has infinitely many ones in both directions. The lecture lower-bound theorem states

$$
\operatorname{SCI}(\Xi_{\rm col})_G=3,
$$

even for unrestricted general algorithms.

For a zero-one sequence $a=(a_i)_{i\in\mathbb Z}$, define $B_a$ on $\ell^2(\mathbb Z)$ to be the identity on coordinates where $a_i=0$ and the shift from each coordinate with $a_i=1$ to the next coordinate carrying a one. It is a direct sum of identity pieces and one shift chain. Consequently:

- finitely many ones give $\operatorname{Sp}(B_a)\subset\{0,1\}$;
- infinitely many ones in both directions give the unit circle $\mathbb T$;
- a one-sided infinite sequence gives the closed unit disk $\overline{\mathbb D}$.

For the columns $a^{(j)}=(a_{ij})_i$, form the bounded direct-sum operator

$$
C(a)=\bigoplus_{j\in\mathbb Z}B_{a^{(j)}}.
$$

Every finite set of matrix entries of $C(a)$ is determined by finitely many entries of $a$, so this construction respects the finite-information condition for a [general algorithm in the SCI hierarchy](../../../../../../general-algorithm-in-the-sci-hierarchy.md). The preceding trichotomy implies

$$
\Xi_{\rm col}(a)=\mathrm{No}
\quad\Longrightarrow\quad
\operatorname{Sp}(C(a))=\overline{\mathbb D},
$$

whereas

$$
\Xi_{\rm col}(a)=\mathrm{Yes}
\quad\Longrightarrow\quad
\operatorname{Sp}(C(a))\subset\{0\}\cup\mathbb T.
$$

The two cases are separated by the point $1/2$: its distance from the spectrum is respectively zero and $1/2$.

If a height-two tower $\Gamma_{n_2,n_1}$ computed the spectrum of every bounded operator, apply it to $C(a)$ and inspect

$$
\alpha_{n_2,n_1}
=\operatorname{dist}\!\left(\frac12,\Gamma_{n_2,n_1}(C(a))\right).
$$

Use the disjoint intervals $[0,1/8]$ and $[3/8,\infty)$ to turn each finite output into Yes or No, retaining the latest inner-stage value that lies in either interval. Convergence in the [Hausdorff distance](../../../../../../hausdorff-distance.md) ensures that the inner limit stabilizes; the outer limit answers $\Xi_{\rm col}$ correctly. This would give a height-two tower for a problem whose [Solvability complexity index](../../../../../../solvability-complexity-index.md) is three, a contradiction. Therefore

$$
\boxed{\operatorname{SCI}(\operatorname{Sp},
\mathcal B(\ell^2(\mathbb N)))\geq3.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
