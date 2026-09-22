<h1 id="18c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\kappa=|k|>0$. Profiles satisfying the rigid-wall conditions are

$$
\varphi_1=A_1\cosh[\kappa(y-h_1)]e^{i(kx-\omega t)},\qquad
\varphi_2=A_2\cosh[\kappa(y+h_2)]e^{i(kx-\omega t)}.
$$

The kinematic conditions at zero give

$$
A_1=\frac{i\omega\eta_0}{\kappa\sinh(\kappa h_1)},\qquad
A_2=-\frac{i\omega\eta_0}{\kappa\sinh(\kappa h_2)}.
$$

Consequently $\varphi_{1t}(0)$ has amplitude $\omega^2\eta_0\coth(\kappa h_1)/\kappa$, whereas $\varphi_{2t}(0)$ has amplitude $-\omega^2\eta_0\coth(\kappa h_2)/\kappa$. Substituting into the dynamic condition yields the [dispersion relation for interfacial gravity waves between rigid boundaries](../../../../../../dispersion-relation-for-interfacial-gravity-waves-between-rigid-boundaries.md):

$$
\boxed{\omega^2=\frac{g(\rho_2-\rho_1)|k|}
{\rho_1\coth(|k|h_1)+\rho_2\coth(|k|h_2)}.}
$$

It is positive because the heavier fluid is below. As $k\to0$, $\omega^2\sim g(\rho_2-\rho_1)k^2/(\rho_1/h_1+\rho_2/h_2)$, while in the deep-layer limit it becomes $g(\rho_2-\rho_1)|k|/(\rho_1+\rho_2)$. The spatially uniform mode has zero restoring frequency.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18C](../../18c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
