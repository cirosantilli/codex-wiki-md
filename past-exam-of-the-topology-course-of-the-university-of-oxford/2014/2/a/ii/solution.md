<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First assume **both factors are nonempty**. If the product is [compact](../../../../../compact-space.md), its [continuous](../../../../../continuous-function.md) coordinate projections are onto, so each factor is [compact](../../../../../compact-space.md) by the [continuous image of a compact space](../../../../../continuous-image-of-a-compact-space.md) theorem.

For the converse, let $X,Y$ be [compact](../../../../../compact-space.md) and let $(W_\lambda)$ be an [open](../../../../../open-set.md) cover of their product. Fix $x\in X$. For every $y\in Y$, choose a [basis](../../../../../basis.md) rectangle $U_{x,y}\times V_{x,y}$ containing $(x,y)$ and lying in a cover member $W_{\lambda(x,y)}$. [Compactness](../../../../../compact-space.md) of $Y$ gives finitely many $V_{x,y_j}$ covering $Y$. Then

$$
U_x=\bigcap_jU_{x,y_j}
$$

is an [open neighbourhood](../../../../../open-neighbourhood.md) of $x$, and $U_x\times Y$ is covered by the corresponding finitely many $W_{\lambda(x,y_j)}$.

The sets $U_x$ cover $X$. [Compactness](../../../../../compact-space.md) gives finitely many of them covering $X$, and the finitely many cover members associated to these choices now cover $X\times Y$. Hence the product is [compact](../../../../../compact-space.md). This is the finite-product [Tychonoff theorem](../../../../../tychonoff-s-theorem.md) proof, with the [finite intersection](../../../../../finite-intersection.md) creating a uniform neighbourhood along each fibre.

As printed, the assertion omits the nonempty hypothesis. If $X=\varnothing$ and $Y=\mathbb R$, the product is [compact](../../../../../compact-space.md) while $Y$ is not. The fully correct version without any nonemptiness assumption is

$$
\boxed{X\times Y\text{ compact}\iff X=\varnothing\text{ or }Y=\varnothing\text{ or both factors are compact}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
