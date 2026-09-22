<h1 id="37a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
L=-mc\sqrt{-\dot x^2}+qA_\nu(x)\dot x^\nu.
$$

Since

$$
\sqrt{-\dot x^2}=c\frac{d\tau}{d\lambda},
\qquad
\dot x^\mu=\frac{d\tau}{d\lambda}u^\mu,
$$

its derivatives are

$$
\frac{\partial L}{\partial\dot x^\mu}
=m u_\mu+qA_\mu,
\qquad
\frac{\partial L}{\partial x^\mu}
=q(\partial_\mu A_\nu)\dot x^\nu.
$$

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) therefore gives

$$
\begin{aligned}
0
&=\frac d{d\lambda}(m u_\mu+qA_\mu)
-q(\partial_\mu A_\nu)\dot x^\nu\\
&=m\frac{du_\mu}{d\lambda}
+q(\partial_\nu A_\mu-\partial_\mu A_\nu)\dot x^\nu.
\end{aligned}
$$

Using the [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md)

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu
$$

and dividing by $d\tau/d\lambda$ gives

$$
\boxed{
m\frac{du_\mu}{d\tau}=qF_{\mu\nu}u^\nu
}.
$$

Raising the first index yields the equivalent requested form

$$
\boxed{
m\frac{du^\mu}{d\tau}=qF^{\mu\nu}u_\nu
}.
$$

This is the [Lorentz-force equation from the worldline action](../../../../../../lorentz-force-equation-from-the-worldline-action.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [37A](../../37a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
