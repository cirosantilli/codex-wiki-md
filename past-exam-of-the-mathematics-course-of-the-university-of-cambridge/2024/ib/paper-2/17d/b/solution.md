<h1 id="17d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A differential equation is stiff when it contains rapidly decaying modes on time scales much shorter than those of interest, forcing an explicit method to take very small steps for stability rather than accuracy.

Here

$$
\det(\lambda I-M)=\lambda^2+101\lambda+100
=(\lambda+1)(\lambda+100),
$$

so the decay rates are $1$ and $100$. For a negative real [eigenvalue](../../../../../../eigenvalue.md), forward Euler requires

$$
|1+h\lambda|\leq1,
$$

therefore the fast mode imposes

$$
\boxed{0<h\leq\frac2{100}=0.02}.
$$

For backward Euler the amplification factors are

$$
\frac1{1-h\lambda}=\frac1{1+h|\lambda|},
$$

whose [moduli](../../../../../../modulus.md) are at most one for every $h\geq0$. Thus

$$
\boxed{\text{backward Euler has no stability upper bound on }h}.
$$

This is the [stiff two-mode linear system](../../../../../../stiff-two-mode-linear-system.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17D](../../17d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
