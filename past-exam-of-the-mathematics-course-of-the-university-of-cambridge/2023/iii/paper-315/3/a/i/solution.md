<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
A=\rho_c+\rho_m,
\qquad
b=\frac{\rho_m}{R_c},
\qquad
d=\frac{\rho_mR_c^3}{12}.
$$

The [enclosed mass](../../../../../../../enclosed-mass.md) is

$$
m(r)=
\begin{cases}
\dfrac{4\pi}{3}\rho_cr^3,&0\leq r\leq R_c,\\
4\pi\left(\dfrac{Ar^3}{3}-\dfrac{br^4}{4}-d\right),&R_c\leq r\leq R_p.
\end{cases}
$$

This is continuous at the core boundary. [Hydrostatic equilibrium](../../../../../../../hydrostatic-equilibrium.md) gives $dP/dr=-Gm(r)\rho(r)/r^2$, with $P(R_p)=0$. Define

$$
F(r)=4\pi G\left(
\frac{A^2r^2}{6}
-\frac{7Abr^3}{36}
+\frac{b^2r^4}{16}
+bd\log(r/R_c)
+\frac{Ad}{r}
\right).
$$

Since $F'(r)=Gm(r)(A-br)/r^2$, the mantle pressure is

$$
\boxed{P(r)=F(R_p)-F(r),
\qquad R_c\leq r\leq R_p}.
$$

Inside the uniform core, the [shell theorem](../../../../../../../spherical-shell-theorem.md) gives $m(r)=4\pi\rho_cr^3/3$, so

$$
\boxed{
P(r)=F(R_p)-F(R_c)
+\frac{2\pi G\rho_c^2}{3}(R_c^2-r^2),
\qquad 0\leq r\leq R_c}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
