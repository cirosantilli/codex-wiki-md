<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The test accepts $P$ when $D(\widehat P_n\Vert P)\leq\delta$. Under $P$, the [method of types](../../../../../../method-of-types.md) gives

$$
e_1^{(n)}
\leq(n+1)^{|A|}2^{-n\delta},
$$

so

$$
D_1(\delta)=\delta.
$$

Under $Q$, accepting $P$ requires a type in the closed set $\{R:D(R\Vert P)\leq\delta\}$. Therefore

$$
e_2^{(n)}
\leq(n+1)^{|A|}2^{-nD_2(\delta)},
$$

where

$$
D_2(\delta)
=\min_{R:D(R\Vert P)\leq\delta}D(R\Vert Q).
$$

Consequently $\limsup_n n^{-1}\log_2e_i^{(n)}\leq-D_i(\delta)$ for $i=1,2$. The first exponent is positive when $\delta>0$. Because relative entropy vanishes only when its arguments agree, the second is positive exactly while $Q$ lies outside the constraint set. Thus both are strictly positive for

$$
\boxed{0<\delta<D(Q\Vert P).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
