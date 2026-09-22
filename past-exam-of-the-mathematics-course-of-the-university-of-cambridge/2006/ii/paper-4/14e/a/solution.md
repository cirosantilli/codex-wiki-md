<h1 id="14e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose $F(z)=(z+1)^{1/3}z^{1/3}(z-1)^{1/3}$, each factor initially defined by polar argument in $(-\pi,\pi)$. The products of the boundary values agree on $(-\infty,-1)$, so their apparent cuts there cancel; the product extends analytically to $\mathbb C\setminus[-1,1]$ and has $F(z)\sim z$ at infinity. In polar coordinates about the three [branch points](../../../../../../branch-point.md) this choice is $\prod r_j^{1/3}\exp[i\sum\theta_j/3]$.

For $0<x<1$, its upper and lower bank values are $e^{\pm i\pi/3}[x(1-x^2)]^{1/3}$. For $-1<x<0$ they are $e^{\pm2i\pi/3}[(-x)(1-x^2)]^{1/3}$. The upper-minus-lower jump on each half is therefore $2i\sin(\pi/3)$ times the positive real integrand. Deforming a positively oriented large circle onto the cut, with the upper bank traversed right to left, gives

$$
\oint F(z)dz=-4i\sin(\pi/3)I.
$$

Small circles about the [branch points](../../../../../../branch-point.md) contribute zero in the limit. At infinity,

$$
F(z)=z(1-z^{-2})^{1/3}=z-\frac1{3z}+O(z^{-3}),
$$

so the large-circle integral is $-2\pi i/3$. Hence

$$
\boxed{I=\frac{\pi}{6\sin(\pi/3)}}.
$$

Both the branch choice and the orientation are essential to the sign.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14E](../../14e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
