<h1 id="20/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Minimize the squared distance $F=x^2+y^2$, which has the same minimizers as the distance. The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations for the constraint $G=x^2+xy-1=0$ are

$$
2x=\lambda(2x+y),\qquad 2y=\lambda x,\qquad x^2+xy=1.
$$

The constraint [gradient](../../../../../../gradient.md) cannot vanish on this branch, since its second component is $x>0$. Eliminate $\lambda=2y/x$ to obtain $x^2=2xy+y^2$. Put $t=y/x$; then $t^2+2t-1=0$, so $t=-1\pm\sqrt2$. But the constraint says $x^2(1+t)=1$, requiring $1+t>0$ and selecting $t=\sqrt2-1$. It follows that

$$
\boxed{(x,y)=\left(2^{-1/4},(\sqrt2-1)2^{-1/4}\right),\qquad
 d_{\min}=\sqrt{2(\sqrt2-1)}.}
$$

To prove a [global minimum](../../../../../../global-minimum.md) on the whole $x>0$ branch, substitute $y=1/x-x$ into $F$:

$$
F=2x^2+x^{-2}-2\geq2\sqrt2-2.
$$

The [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) proves this bound, with equality only when $2x^2=x^{-2}$, namely $x=2^{-1/4}$. Thus the [stationary point](../../../../../../stationary-point.md) is the unique closest point on the required branch. Numerically it is approximately $(0.840896,0.348311)$ and its distance is $0.910180$ in coordinate units.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [20](../../../20.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
