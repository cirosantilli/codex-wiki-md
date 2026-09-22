<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The complex [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) says that every bounded complex-[linear functional](../../../../linear-functional.md) on a [linear subspace](../../../../vector-subspace.md) of a normed complex space extends to the whole space with the same [norm](../../../../norm.md).

For the separation assertion choose $x_0\notin M$ and $d=\operatorname{dist}(x_0,M)>0$. On $M+\mathbb Cx_0$ define $g_0(m+\lambda x_0)=\lambda d$. The inequality $\|m+\lambda x_0\|\geq|\lambda|d$ makes its [norm](../../../../norm.md) at most one; approximating the distance $d$ shows the [norm](../../../../norm.md) is exactly one. Hahn-Banach gives an extension $g$ of [norm](../../../../norm.md) one annihilating $M$.

Each [geometric sequence](../../../../geometric-progression.md) satisfies $\|x_k\|_1=(1-|\beta_k|)^{-1}\leq(1-\delta)^{-1}$. Let $M$ be their [closed linear span](../../../../closed-linear-span.md). If $M\ne\ell^1$, the separation just proved gives a nonzero bounded functional annihilating all $x_k$. Represent it by $b\in\ell^\infty$ and form

$$
F(z)=\sum_{j=1}^\infty b_jz^{j-1},\qquad|z|<1.
$$

The series converges locally uniformly and defines a [holomorphic function](../../../../holomorphic-function-split.md). It vanishes at every $\beta_k$. These distinct points lie in the [compact](../../../../compact-space.md) disk $|z|\leq\delta<1$, so have an accumulation point inside the domain. The [identity theorem](../../../../identity-theorem.md) gives $F=0$, hence every [Taylor coefficient](../../../../taylor-coefficient.md) $b_j=0$, contradicting the functional's nonzero [norm](../../../../norm.md). Therefore

$$
\boxed{\overline{\operatorname{span}\{x_k:k\geq1\}}=\ell^1.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
