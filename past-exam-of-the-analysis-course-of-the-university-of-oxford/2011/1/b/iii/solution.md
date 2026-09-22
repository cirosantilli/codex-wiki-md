<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $q(x)=\sup_k|\sum_{n=1}^kx_n|$. This is indeed a [norm](../../../../../norm.md): the [triangle inequality](../../../../../triangle-inequality.md) and homogeneity follow from the scalar absolute value, and vanishing of every [partial sum](../../../../../partial-sum.md) forces every coordinate to vanish. It is finite on $\ell^1$ because $q(x)\leq\|x\|_1$.

Let $a_n=(-1)^{n+1}/n$ and let $a^{(N)}$ be its first $N$ entries followed by zeros. The alternating-[series](../../../../../series-mathematics.md) bound gives, for $M>N$,

$$
q(a^{(M)}-a^{(N)})\leq\frac1{N+1}.
$$

Thus these truncations are Cauchy for $q$. But $|x_n|\leq2q(x)$ for every coordinate, since $x_n$ is the difference of two consecutive [partial sums](../../../../../partial-sum.md). Any $q$-limit would consequently have coordinates $a_n$. This sequence is not in $\ell^1$. Hence

$$
\boxed{(\ell^1,q)\text{ is not a Banach space}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
