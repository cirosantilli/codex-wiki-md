<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [volumetric flow rate](../../../../../../volumetric-flow-rate.md) is $Q=2\pi\int_0^R u(r)r\,dr$. [Integration by parts](../../../../../../integration-by-parts.md), using finite $u(0)$ and $u(R)=0$, gives

$$
Q=-\pi\int_0^Rr^2\frac{du}{dr}\,dr
=\boxed{\pi\int_0^R\dot\gamma(r)r^2\,dr}.
$$

Because the stress magnitude is $\tau=\tau_Rr/R$, change variables from $r$ to $\tau$:

$$
\boxed{Q=\frac{\pi R^3}{\tau_R^3}
\int_0^{\tau_R}\dot\gamma(\tau)\tau^2\,d\tau}.
$$

Therefore the required power is $n=3$. The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives the pipe form of the [Weissenberg–Rabinowitsch equation](../../../../../../weissenberg-rabinowitsch-equation.md):

$$
\boxed{\dot\gamma_R
=\frac1{\pi R^3\tau_R^2}
\frac d{d\tau_R}(Q\tau_R^3)
=\frac{3Q+\tau_R,dQ/d\tau_R}{\pi R^3}}.
$$

Finally $\eta(\dot\gamma_R)=\tau_R/\dot\gamma_R$, so

$$
\boxed{\eta(\dot\gamma_R)
=\frac{\pi R^3\tau_R}
{3Q+\tau_R,dQ/d\tau_R}}.
$$

A measured pressure-drop--flow-rate curve therefore recovers the wall viscosity without assuming a constitutive form.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
