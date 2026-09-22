<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For a Boolean-valued $f$, each [discrete derivative of a Boolean function](../../../../../../discrete-derivative-of-a-boolean-function.md) $D_i f$ takes values in $\{-1,0,1\}$ and has degree at most $k-1$. If $f$ depends on coordinate $i$, then $D_i f$ is nonzero, so part (iii) gives

$$
\operatorname{Inf}_i(f)=\mathbb E(D_i f)^2
=\mathbb P[D_i f\ne0]\geq2^{-(k-1)}.
$$

Since $f$ has degree at most $k$, the Fourier formula for [total influence](../../../../../../total-influence.md) and [Parseval identity](../../../../../../parseval-identity.md) give

$$
\mathbf I(f)=\sum_S|S|\widehat f(S)^2
\leq k\sum_S\widehat f(S)^2=k.
$$

If $m$ coordinates affect $f$, then $m2^{-(k-1)}\leq\mathbf I(f)\leq k$, so $m\leq k2^{k-1}$. Thus $f$ is a $k2^{k-1}$-[junta](../../../../../../junta.md), which is the [Nisan-Szegedy junta theorem](../../../../../../nisan-szegedy-junta-theorem.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
