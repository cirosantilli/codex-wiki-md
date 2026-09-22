<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take steady simple shear $u_x=\dot\gamma y$ and define $W_i=\lambda_i\dot\gamma$. Substitution of the symmetric stress components into the full constitutive equation gives, after solving the three coupled algebraic equations,

$$
\tau_{xy}=\eta\dot\gamma
\frac{1+a(2-a)W_1W_2}{1+a(2-a)W_1^2}.
$$

Thus the [Steady shear viscosity of a Johnson--Segalman--Oldroyd fluid](../../../../../../steady-shear-viscosity-of-a-johnson-segalman-oldroyd-fluid.md) is

$$
\boxed{\eta_{\rm sh}(\dot\gamma)
=\frac{\tau_{xy}}{\dot\gamma}
=\eta\frac{1+a(2-a)\lambda_1\lambda_2\dot\gamma^2}
{1+a(2-a)\lambda_1^2\dot\gamma^2}.}
$$

For the stated small positive $a$, so that $0<a<2$, this decreases from $\eta$ at zero rate to $\eta\lambda_2/\lambda_1$ at high rate exactly when

$$
\boxed{\lambda_1>\lambda_2.}
$$

Equality gives constant viscosity, while $\lambda_2>\lambda_1$ gives shear thickening.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
