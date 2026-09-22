<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take distinct $x,y\in A_n$. Their difference has the form

$$
x-y=P(\alpha),
$$

where $P\in\mathbb Z[X]$ has degree at most $n-1$ and [polynomial length](../../../../../../polynomial-length.md) at most $nh$. By the [height bound for a polynomial evaluation](../../../../../../height-bound-for-a-polynomial-evaluation.md),

$$
H(x-y)\leq nh\,H(\alpha)^{n-1}.
$$

The algebraic number $x-y$ is nonzero and has degree at most $d$, so the [Liouville height inequality](../../../../../../liouville-height-inequality.md) gives the separation

$$
|x-y|
\geq(nh)^{-d}H(\alpha)^{-d(n-1)}.
$$

All elements of $A_n$ lie in an interval of length at most

$$
\frac h{1-\alpha}.
$$

Since $H(1-\alpha)\leq2H(\alpha)$, another application of the [Liouville height inequality](../../../../../../liouville-height-inequality.md) gives

$$
\frac1{1-\alpha}\leq(2H(\alpha))^d.
$$

The number of points in an interval is at most one plus its length divided by their minimum separation. Consequently

$$
|A_n|
\leq
2^dh(nh)^dH(\alpha)^{dn}+1
\leq
(2hn)^{d+1}H(\alpha)^{dn}+1.
$$

**Thus the requested statement holds, for example, with the absolute constant $C=2$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
