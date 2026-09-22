<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $n\le x$, write $F(n)=F(x)-\int_n^xF'(t)dt$, multiply by $f(n)$ and sum. Interchanging a finite sum with the [integral](../../../../integral-split.md) gives the [Abel summation formula](../../../../abel-s-summation-formula.md)

$$
\sum_{n\le x}f(n)F(n)=S(x)F(x)-\int_1^xS(t)F'(t)\,dt.
$$

Apply it with $F(t)=t^{-s}$ and $S(t)=\sum_{n\le t}a_n$. If $\sigma>\alpha$, the boundary term is $O(x^{\alpha-\sigma})\to0$ and $\int_1^\infty|S(t)t^{-s-1}|dt$ converges. Therefore the [Dirichlet series](../../../../dirichlet-series.md) converges and

$$
A(s)=s\int_1^\infty S(t)t^{-s-1}dt=s\sum_{m\ge1}I_m(s).
$$

Choose $C$ with $|S(t)|\le Ct^\alpha$ for $t\ge1$. For $\sigma>\alpha+\delta$,

$$
|I_m(s)|\le C\int_m^{m+1}t^{\alpha-\sigma-1}dt\le Cm^{-1-\delta}.
$$

The [Weierstrass M-test](../../../../weierstrass-m-test.md) proves [uniform convergence](../../../../uniform-convergence.md) of $\sum I_m$ on this entire open half-plane. For fixed $s$, the same estimate with its actual $\sigma$ gives $I_m(s)=O(m^{\alpha-1-\sigma})$. Each $I_m$ is an [entire function](../../../../entire-function.md), since its [integral](../../../../integral-split.md) has bounded positive $t$ range and can be differentiated in $s$ under an integrable bound on each [compact set](../../../../compact-space.md). Thus the locally uniform sum is [holomorphic](../../../../holomorphic-function-split.md), and so is its product with $s$. This gives [holomorphy from polynomial growth of arithmetic partial sums](../../../../holomorphy-from-polynomial-growth-of-arithmetic-partial-sums.md) and proves holomorphy of $A$ for $\operatorname{Re}s>\alpha$. Multiplication by the unbounded factor $s$ does not assert [uniform convergence](../../../../uniform-convergence.md) of $A$ on a whole unbounded half-plane; local [uniform convergence](../../../../uniform-convergence.md) is what the holomorphy argument needs.

With $a_n=\mu(n)$ and the hypothetical bound, $A_\mu(s)$ is [holomorphic](../../../../holomorphic-function-split.md) for $\operatorname{Re}s>3/4$. On $\operatorname{Re}s>1$, the [Euler product](../../../../euler-product.md) gives $\zeta(s)A_\mu(s)=1$. The [identity theorem](../../../../identity-theorem.md) extends this as a meromorphic identity throughout the connected half-plane $\operatorname{Re}s>3/4$. Hence $\zeta$ has **no zeros in that half-plane**: at any zero, the product with the [holomorphic](../../../../holomorphic-function-split.md) $A_\mu$ would be zero. The [pole](../../../../pole.md) at one is not a zero; $A_\mu$ has a compensating zero there.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
