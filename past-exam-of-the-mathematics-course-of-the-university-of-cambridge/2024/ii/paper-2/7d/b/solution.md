<h1 id="7d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x>0$, take the real contour $\gamma=(-\infty,0)$. At $t\to0^-$ the factor $e^{-1/t^2}$ kills every power, while at $t\to-\infty$ the factor $e^{xt}$ makes the integrand and endpoint term vanish. The [laplace integral solution of a singular third-order equation](../../../../../../laplace-integral-solution-of-a-singular-third-order-equation.md) is therefore

$$
y(x)=C\int_{-\infty}^0 e^{xt-1/t^2}t^{-3}\,dt.
$$

With $u=-1/t$, and absorbing a minus sign into the arbitrary constant, this becomes

$$
\boxed{y(x)=C_1\int_0^\infty u\exp\left(-u^2-\frac xu\right)du}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7D](../../7d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
