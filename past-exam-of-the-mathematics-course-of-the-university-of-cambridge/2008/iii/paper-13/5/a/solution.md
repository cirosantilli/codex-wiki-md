<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Recall that $g_i\in L^1_{\mathrm{loc}}(\Omega)$ is the [weak derivative](../../../../../../weak-derivative.md) $D_i u$ if $u\in L^1_{\mathrm{loc}}(\Omega)$ and $\int uD_i\phi=-\int g_i\phi$ for all $\phi\in C_c^\infty(\Omega)$. A global [weak derivative](../../../../../../weak-derivative.md) restricts to every open neighborhood simply by taking [test functions](../../../../../../test-function.md) supported there.

Conversely, suppose local [weak derivatives](../../../../../../weak-derivative.md) exist near each point. [local integrability](../../../../../../locally-integrable-function.md) of $u$ follows by a finite cover of each compact subset. On overlapping neighborhoods the two candidates for $D_i u$ have identical integrals against every smooth compactly supported [test function](../../../../../../test-function.md). The fundamental lemma for [locally integrable](../../../../../../locally-integrable-function.md) functions therefore makes them equal [almost everywhere](../../../../../../almost-everywhere.md). Choose a countable local cover, possible in Euclidean space; the countably many exceptional overlap sets can all be discarded. The derivatives consequently patch to measurable $g_i\in L^1_{\mathrm{loc}}(\Omega)$.

For a [test function](../../../../../../test-function.md) $\phi$, take a smooth [partition of unity](../../../../../../partition-of-unity.md) $(\chi_j)$ subordinate to the local cover and locally finite on its support. Only finitely many terms occur there. Because $\sum_j\chi_j=1$ near the support,

$$
\int_\Omega uD_i\phi=\sum_j\int_\Omega uD_i(\chi_j\phi)
=-\sum_j\int_\Omega g_i\chi_j\phi=-\int_\Omega g_i\phi.
$$

The derivatives of the partition sum to zero, explaining the first equality. Thus the patched functions are the global [weak derivatives](../../../../../../weak-derivative.md). This proves both directions of [locality of weak differentiability](../../../../../../locality-of-weak-differentiability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
