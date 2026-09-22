<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $c=\cos(\alpha\xi_3)$, $s=\sin(\alpha\xi_3)$ and $r^2=x_1^2+x_2^2=(\xi_1^2+\xi_2^2)/\lambda$. Differentiating the deformation gives

$$
A=\begin{pmatrix}
\lambda^{-1/2}c&-\lambda^{-1/2}s&-\alpha x_2\\
\lambda^{-1/2}s&\lambda^{-1/2}c&\alpha x_1\\
0&0&\lambda
\end{pmatrix},
\qquad \det A=1.
$$

For the [neo-Hookean solid](../../../../../neo-hookean-solid.md), $W_{,A_{i\alpha}}=\mu A_{i\alpha}$. The constrained [nominal stress tensor](../../../../../nominal-stress-tensor.md) is therefore $N_{\alpha i}=\mu A_{i\alpha}+q(A^{-1})_{\alpha i}$. The multiplier cannot be set arbitrarily to a constant; equilibrium and the traction-free curved surface determine it.

Push the [nominal stress](../../../../../nominal-stress-tensor.md) to the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md): since $J=1$, $\sigma=AN=\mu AA^T+qI$. In the current cylindrical orthonormal basis, the [left Cauchy-Green deformation tensor](../../../../../left-cauchy-green-deformation-tensor.md) has entries

$$
AA^T=\begin{pmatrix}
\lambda^{-1}&0&0\\
0&\lambda^{-1}+\alpha^2r^2&\alpha\lambda r\\
0&\alpha\lambda r&\lambda^2
\end{pmatrix}.
$$

Thus $\sigma_{rr}=\mu/\lambda+q$, $\sigma_{\vartheta\vartheta}=\mu/\lambda+\mu\alpha^2r^2+q$, and $\sigma_{\vartheta3}=\mu\alpha\lambda r$. Static radial equilibrium without [body force](../../../../../body-force.md) gives

$$
\frac{d\sigma_{rr}}{dr}+\frac{\sigma_{rr}-\sigma_{\vartheta\vartheta}}r=0,
\qquad q'(r)=\mu\alpha^2r.
$$

The current outer radius is $a=R/\sqrt\lambda$. Setting $\sigma_{rr}(a)=0$ integrates the reaction field:

$$
\boxed{q(r)=-\frac\mu\lambda+\frac{\mu\alpha^2}{2}(r^2-a^2).}
$$

The other curved-surface [traction](../../../../../traction.md) components vanish because $\sigma_{r\vartheta}=\sigma_{r3}=0$.

On the reference end $\xi_3=H$, the outward reference normal is $e_3$, and the nominal [traction](../../../../../traction.md) has components $t_i=N_{3i}$. The third row of $A^{-1}$ is $(0,0,\lambda^{-1})$. Hence the [nominal end traction of a twisted neo-Hookean cylinder](../../../../../nominal-end-traction-of-a-twisted-neo-hookean-cylinder.md) is

$$
\boxed{\begin{aligned}
t_1&=-\mu\alpha x_2,\\
t_2&=\mu\alpha x_1,\\
t_3&=\mu(\lambda-\lambda^{-2})
+\frac{\mu\alpha^2}{2\lambda^2}(\xi_1^2+\xi_2^2-R^2).
\end{aligned}}
$$

The current $x_1,x_2$ here are evaluated at $\xi_3=H$. These components are per unit reference area, not per unit current area.

For the moment, use current lever arms and reference-area [traction](../../../../../traction.md). Its axial component is

$$
\begin{aligned}
M_3&=\int_{\xi_1^2+\xi_2^2<R^2}(x_1t_2-x_2t_1)\,d\xi_1d\xi_2\\
&=\frac{\mu\alpha}{\lambda}\int_0^{2\pi}\int_0^R s^2s\,ds\,d\vartheta
=\boxed{\frac{\mu\pi R^4\alpha}{2\lambda}.}
\end{aligned}
$$

The axial [traction](../../../../../traction.md) gives no axial moment. This [torque](../../../../../torque.md) also agrees with the reference-energy derivative at fixed axial stretch: the twist-dependent energy per reference length is $\mu\alpha^2\pi R^4/(4\lambda)$. It is important that $\alpha$ is twist per reference length, not twist per current length.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
