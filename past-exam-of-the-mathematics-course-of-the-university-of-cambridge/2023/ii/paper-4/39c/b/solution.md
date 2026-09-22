<h1 id="39c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work in the [shock frame](../../../../../../shock-frame.md), and let the positive upstream and downstream speeds be $w_0$ and $w_1$. The [Rankine-Hugoniot conditions for a perfect gas](../../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) give conservation of mass and momentum:

$$
\rho_0w_0=\rho_1w_1,
\qquad
p_0+\rho_0w_0^2=p_1+\rho_1w_1^2.
$$

Put

$$
r=\frac{\rho_1}{\rho_0},\qquad
\frac{p_1}{p_0}=1+\beta.
$$

Mass conservation gives $w_1=w_0/r$, and momentum conservation then gives

$$
w_0^2=\frac{p_0}{\rho_0}\frac{\beta r}{r-1}. \qquad (1)
$$

Applying the energy integral from part (a) on the two sides gives

$$
\frac{\gamma}{\gamma-1}\frac{p_0}{\rho_0}+\frac12w_0^2
=\frac{\gamma}{\gamma-1}\frac{p_0(1+\beta)}{\rho_0r}
+\frac12\frac{w_0^2}{r^2}. \qquad (2)
$$

Substitution of (1) into (2), followed by cancellation of $p_0/\rho_0$, yields

$$
\frac{\beta(r+1)}2
=\frac{\gamma}{\gamma-1}(1+\beta-r).
$$

Solving this linear equation for the density ratio gives

$$
\boxed{\frac{\rho_1}{\rho_0}=r
=\frac{2\gamma+(\gamma+1)\beta}
{2\gamma+(\gamma-1)\beta}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
