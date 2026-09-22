<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Boolean function](../../../../../../boolean-function.md) $f:\{0,1\}^n\to\{0,1\}$ is [$(\varepsilon,p,r)$-quasirandom](../../../../../../quasirandom-boolean-function.md) when, for every $J\subseteq[n]$ with $|J|\leq r$ and every $u\in\{0,1\}^J$,

$$
\left|\mathbb E_{\mu_p}[f\mid x|_J=u]-\mathbb E_{\mu_p}f\right|\leq\varepsilon.
$$

The [regularity lemma for Boolean functions](../../../../../../regularity-lemma-for-boolean-functions.md) states that for every $\varepsilon,p,r,\delta$ there is $T$ such that every Boolean function has a set $J$, $|J|\leq T$, for which a $\mu_p$-random $u\in\{0,1\}^J$ satisfies

$$
\mathbb P_u[f_u\text{ is }(\varepsilon,p,r)\text{-quasirandom}]\geq1-\delta.
$$

Here $f_u$ is the restriction obtained by fixing the coordinates in $J$ to $u$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
