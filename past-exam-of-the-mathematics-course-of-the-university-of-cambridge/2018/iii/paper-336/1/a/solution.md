<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the [square root](../../../../../../square-root.md) with $-\pi/2<\arg z<3\pi/2$, so the [branch cut](../../../../../../branch-cut.md) is the negative imaginary axis. The change of variable $u=e^{-i\pi/4}\sqrt z$ maps this sheet onto $\operatorname{Re}u>0$ and gives $z=iu^2$. Writing the [exponential function](../../../../../../exponential-function.md) as $e^{k\phi(z)}$, its phase becomes exactly quadratic:

$$
\phi(z)=-i\bigl(z-2e^{i\pi/4}\sqrt z\bigr)=(u-1)^2-1.
$$

The [saddle point](../../../../../../saddle-point.md) is therefore $u=1$, or **$z_s=i$**. On the descending line $u=1+iv$, $v\in\mathbb R$, the phase is $-1-v^2$. Its image is the [parabola](../../../../../../parabola.md)

$$
\boxed{z=-2v+i(1-v^2),\qquad\operatorname{Im}z=1-\frac{(\operatorname{Re}z)^2}{4}.}
$$

The contour runs from left to right, corresponding to $v$ decreasing from $+\infty$ to $-\infty$. A [contour deformation](../../../../../../contour-deformation.md) in the right half of the $u$-plane moves the original indented contour to this line. The connecting tails vanish in the descending sectors, and no [branch point](../../../../../../branch-point.md) or [pole](../../../../../../pole.md) is crossed. Since $dz=-2(1+iv)\,dv$, the [Gaussian integral](../../../../../../gaussian-integral.md) and the [odd function](../../../../../../odd-function.md) $ve^{-kv^2}$ give

$$
I=2e^{-k}\int_{-\infty}^{\infty}(1+iv)e^{-kv^2}\,dv
=\boxed{2\sqrt{\frac\pi k}\,e^{-k}}.
$$

Here the [method of steepest descent](../../../../../../method-of-steepest-descent.md) actually gives an exact answer for $k>0$, because the quadratic phase and linear transformed amplitude have no further even correction.

<a id="1/a/image-integration-contours-near-a-saddle-and-a-pole"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336-contours.png)

**[Figure 1](#1/a/image-integration-contours-near-a-saddle-and-a-pole). Integration contours near a saddle and a pole**. The original upper indentation, the saddle contour, and the negative imaginary branch cut. The indentation is exaggerated for visibility.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
