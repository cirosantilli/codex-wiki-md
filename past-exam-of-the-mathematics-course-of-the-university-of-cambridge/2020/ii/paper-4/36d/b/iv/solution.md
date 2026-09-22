<h1 id="36d/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A real transmitted normal wavenumber exists only if

$$
\sin^2\theta_I\leq\frac{\varepsilon_+}{\varepsilon_-},
$$

so the [critical angle for total internal reflection](../../../../../../../critical-angle-for-total-internal-reflection.md) is

$$
\boxed{\theta_I^{\rm cr}=\arcsin\sqrt{\frac{\varepsilon_+}{\varepsilon_-}}}.
$$

For $\theta_I>\theta_I^{\rm cr}$, put

$$
k_x=k_I\cos\theta_I,
\qquad k_z=k_I\sin\theta_I,
\qquad
\kappa=k_I\sqrt{\sin^2\theta_I-\frac{\varepsilon_+}{\varepsilon_-}}.
$$

For incident amplitude $E_0\widehat{\mathbf y}$, the [transverse-electric Fresnel reflection coefficient](../../../../../../../transverse-electric-fresnel-reflection-coefficient.md) and transmission coefficient are

$$
r=\frac{k_x-i\kappa}{k_x+i\kappa},
\qquad
t=1+r=\frac{2k_x}{k_x+i\kappa}.
$$

A boundary-matched solution is

$$
\mathbf E=\begin{cases}
\operatorname{Im}\!\left\{E_0\widehat{\mathbf y}\left[e^{i(k_xx+k_zz-\omega t)}+r e^{i(-k_xx+k_zz-\omega t)}\right]\right\},&x<0,\\
\operatorname{Im}\!\left\{E_0t\widehat{\mathbf y}\,e^{-\kappa x}e^{i(k_zz-\omega t)}\right\},&x>0,
\end{cases}
$$

with each magnetic component obtained from $\mathbf B_X=\mathbf k_X\times\mathbf E_X/\omega$, now using the complex transmitted wavevector $(i\kappa,0,k_z)$. Since $|r|=1$, the wave undergoes [total internal reflection](../../../../../../../total-internal-reflection.md); the transmitted field is an [evanescent wave](../../../../../../../evanescent-wave.md) that propagates parallel to the interface and decays exponentially into $x>0$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [36D](../../../36d.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
