<h1 id="15e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the half-plane metric is a [conformal rescaling](../../../../../../conformal-rescaling-of-a-riemannian-metric.md) of the Euclidean metric, its angles are Euclidean angles. For each $y>0$, the [hyperbolic lines meeting the imaginary axis at a fixed angle](../../../../../../hyperbolic-lines-meeting-the-imaginary-axis-at-a-fixed-angle.md) $\alpha$ at $iy$ are the Euclidean circles

$$
(x-y\cot\alpha)^2+Y^2=y^2\csc^2\alpha,
$$

where $Y$ denotes the vertical coordinate. These circles have centres on the real axis and are therefore hyperbolic lines; varying $y$ gives the required collection.

To construct a triangle, put one vertex at $i$ and a second at $it$ on $\ell_+$, with $t>1$. Draw from these vertices the lines making interior angles $\alpha$ and $\beta$ with $\ell_+$. Their Euclidean centres and radii are

$$
C_1=\cot\alpha,
\quad R_1=\csc\alpha,
\qquad
C_2=-t\cot\beta,
\quad R_2=t\csc\beta.
$$

If their other intersection has angle $\gamma$, the [law of cosines](../../../../../../law-of-cosines.md) in the Euclidean triangle formed by the two centres and that intersection gives

$$
\cos\gamma
=\frac{R_1^2+R_2^2-(C_1-C_2)^2}{2R_1R_2}
=\frac{\sin\alpha\sin\beta}{2}\left(t+\frac1t\right)-\cos\alpha\cos\beta.
$$

Equivalently,

$$
\frac12\left(t+\frac1t\right)
=\frac{\cos\gamma+\cos\alpha\cos\beta}{\sin\alpha\sin\beta}.
$$

The right side is greater than one exactly when $\alpha+\beta+\gamma<\pi$. Since $(t+t^{-1})/2$ ranges continuously and strictly increasingly from $1$ to infinity for $t>1$, such a $t$ exists. The three lines therefore bound a [hyperbolic triangle](../../../../../../hyperbolic-triangle.md) with the prescribed angles.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15E](../../15e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
