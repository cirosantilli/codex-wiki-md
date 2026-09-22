<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [complex Hahn-Banach theorem](../../../../complex-hahn-banach-theorem.md) extends every bounded complex-[linear functional](../../../../linear-functional.md) on a subspace to the whole normed space with exactly the same [norm](../../../../norm.md). Let $d=\operatorname{dist}(x_0,M)>0$ and define on $M+\mathbb Cx_0$

$$
g_0(y+\lambda x_0)=\lambda d.
$$

The representation is unique. The distance inequality $\|y+\lambda x_0\|\geq|\lambda|d$ gives $\|g_0\|\leq1$. Taking $y=-m$ with $\|x_0-m\|\downarrow d$ proves the reverse [norm](../../../../norm.md) bound. Extend by the [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) to $g\in X'$; then **$g|_M=0$, $\|g\|=1$, and $g(x_0)=d\ne0$**. The labels (a)-(c) specify these simultaneous properties of this one functional.

Let $Y=\overline{\operatorname{span}F}$. Every functional vanishing on $F$ vanishes on $Y$ by linearity and continuity, so $Y\subseteq(F^\circ)_\circ$. If $x\notin Y$, the separation just proved gives a bounded functional zero on $Y$ and nonzero at $x$. It belongs to $F^\circ$ and excludes $x$ from its preannihilator. Therefore

$$
\boxed{(F^\circ)_\circ=\overline{\operatorname{span}F}.}
$$

For the dual-side counterexample take $X=\ell^1$, $X'=\ell^\infty$, and $G=c_0$. It is [norm](../../../../norm.md) closed, since a uniform limit of sequences tending to zero still tends to zero. Every coordinate [unit vector](../../../../unit-vector.md) belongs to $G$, so the only $x\in\ell^1$ annihilated by every element of $G$ has all coordinates zero. Thus $G_\circ=\{0\}$ and

$$
\boxed{(G_\circ)^\circ=\ell^\infty\ne c_0=G.}
$$

The dual-side double annihilator corresponds to weak-star [closure](../../../../closure-topology.md), which need not equal [norm](../../../../norm.md) [closure](../../../../closure-topology.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
