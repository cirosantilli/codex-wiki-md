<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose $0<\alpha<\varepsilon/p$. At dyadic level $m$, [Markov inequality](../../../../../../markov-inequality.md) and a union bound give

$$
\mathbb P\left(\max_k|X^n_{(k+1)2^{-m}}-X^n_{k2^{-m}}|>C2^{-m\alpha}\right)
\leq cC^{-p}2^{-m(\varepsilon-\alpha p)},
$$

uniformly in $n$. Summing over $m$ shows that, outside a set of probability at most $C_0C^{-p}$, all dyadic increments obey this bound. Chaining dyadic approximations and using continuity gives

$$
|X_t^n-X_s^n|\leq C_1C|t-s|^\alpha
$$

for all $s,t$. Since $X_0^n=0$, the paths then lie in the stated compact Hölder set by the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md). Taking $C$ large proves tightness.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
