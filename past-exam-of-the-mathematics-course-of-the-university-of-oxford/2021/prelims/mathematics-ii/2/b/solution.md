<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $u_n=11^n\log n/(2^{2n+1}n!)$ for $n\geq2$. The [factorial](../../../../../../factorial.md) gives

$$
\frac{u_{n+1}}{u_n}=\frac{11}{4(n+1)}\frac{\log(n+1)}{\log n}.
$$

The [logarithm](../../../../../../logarithm.md) identity

$$
\frac{\log(n+1)}{\log n}=1+\frac{\log(1+1/n)}{\log n}\longrightarrow1
$$

follows from [continuity](../../../../../../continuous-function.md) of the [logarithm](../../../../../../logarithm.md) at one and $\log n\to+\infty$. The product rule for [limits of sequences](../../../../../../limit-of-a-sequence.md) therefore makes the displayed ratio tend to zero. In particular, some $N$ satisfies $0<u_{n+1}\leq u_n/2$ for all $n\geq N$. By [mathematical induction](../../../../../../mathematical-induction.md), $0<u_{N+j}\leq u_N2^{-j}$. A [geometric sequence](../../../../../../geometric-progression.md) with ratio in $(0,1)$ tends to zero, so the [squeeze theorem](../../../../../../squeeze-theorem.md) proves

$$
\boxed{\lim_{n\to\infty}\frac{11^n\log n}{2^{2n+1}n!}=0.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
