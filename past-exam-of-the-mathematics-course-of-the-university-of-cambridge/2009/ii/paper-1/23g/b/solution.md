<h1 id="23g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A singular point would satisfy $p=0$, $p_w=2w=0$ and $p_z=-3z^2+2z+1=0$. Thus $w=0$ and $z=1$ or $-1/3$. But $p(1,0)=1$ and $p(-1/3,0)=-5/27$, both nonzero. **The curve is smooth everywhere.**

The complex [implicit function theorem](../../../../../../implicit-function-theorem.md) says that near a zero of a holomorphic function with a nonzero partial derivative, the corresponding variable is a uniquely defined holomorphic function of the others. Where $p_w\ne0$, use $z$ as a local coordinate with $w=w(z)$; where $p_z\ne0$, use $w$ with $z=z(w)$. On overlaps the coordinate transitions are holomorphic with nonzero derivatives. These charts give $Z$ a [Riemann surface](../../../../../../riemann-surfaces.md) structure, and both coordinate projections are [holomorphic](../../../../../../complex-differentiability-at-a-point.md) in them.

A [ramification point](../../../../../../ramification-point-of-a-holomorphic-map.md) of a nonconstant [holomorphic map](../../../../../../holomorphic-map.md) is a point where in local coordinates the map has the form $u\mapsto u^e$ with $e\geq2$; its ramification, or branching, order is $e-1$. For $g=w$, take $(z,w)=(1,i)$. Here $p_w=2i\ne0$, so $z$ is a local coordinate. Differentiating $w(z)^2=z^3-z^2-z$ gives $w'(1)=0$ and $2i w''(1)=4$. Therefore

$$
w(z)-i=\frac1i(z-1)^2+O((z-1)^3).
$$

The nonzero quadratic coefficient gives **local degree $\boxed2$ and branching order $\boxed1$**. If “branching order” denotes local degree rather than its excess in a different convention, the corresponding value is two.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23G](../../23g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
