<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use polar coordinates with $-\pi<\theta<\pi$; the two faces of the screen are $\theta=\pm\pi$. Take $0<\theta_0<\pi$, so the incident wave approaches from the upper half-plane, and retain the specified time dependence $e^{i\omega t}$. Outgoing cylindrical waves then have radial factor $e^{-ik_0r}$. Define the normalized [Fresnel integral](../../../../../../fresnel-integral.md)

$$
\mathcal F(s)=\frac{e^{i\pi/4}}{\sqrt\pi}\int_{-\infty}^{s}e^{-iv^2}\,dv
=\frac12\operatorname{erfc}(-e^{i\pi/4}s),
\qquad s_\pm=\sqrt{2k_0r}\cos\frac{\theta\pm\theta_0}{2}.
$$

The exact Neumann [Sommerfeld half-plane diffraction](../../../../../../sommerfeld-half-plane-diffraction.md) solution for the total spatial field is

$$
\Phi=e^{ik_0r\cos(\theta-\theta_0)}\mathcal F(s_-)
+e^{ik_0r\cos(\theta+\theta_0)}\mathcal F(-s_+),
\qquad \phi=\Phi-\phi_i.
$$

One way to verify the [Helmholtz equation](../../../../../../helmholtz-equation.md) is to use parabolic coordinates $\xi=\sqrt{2r}\cos(\alpha/2)$, $\eta=\sqrt{2r}\sin(\alpha/2)$. Each term has the form $e^{ik_0(\xi^2-\eta^2)/2}\mathcal F(\pm\sqrt{k_0}\xi)$. The operator is $(\xi^2+\eta^2)^{-1}(\partial_\xi^2+\partial_\eta^2)$, and $\mathcal F''(s)+2is\mathcal F'(s)=0$ makes its Helmholtz residual zero. At $\theta=\pm\pi$, the two Fresnel arguments coincide, while the derivatives of both the arguments and plane-wave phases cancel in pairs. Hence $\partial_\theta\Phi=0$, which is the required normal boundary condition.

Away from the Fresnel transition regions, [integration by parts](../../../../../../integration-by-parts.md) gives the [Fresnel tail expansion](../../../../../../fresnel-tail-expansion.md)

$$
\mathcal F(s)=H(s)+\frac{e^{3\pi i/4-is^2}}{2\sqrt\pi\,s}+O(|s|^{-3}),
$$

where $H$ is the [Heaviside step function](../../../../../../heaviside-step-function.md). The same expansion follows from the complementary-error-function asymptotics in [NIST DLMF](https://dlmf.nist.gov/7.12). Because $s_\pm^2=k_0r[1+\cos(\theta\pm\theta_0)]$, the tails in both terms have outgoing phase $e^{-ik_0r}$. The scattered far field is consequently

$$
\boxed{\begin{aligned}
\phi={}&-H(\theta_0-\pi-\theta)e^{ik_0r\cos(\theta-\theta_0)}
+H(\theta-\pi+\theta_0)e^{ik_0r\cos(\theta+\theta_0)}\\
&+\frac{e^{-ik_0r+3\pi i/4}}{\sqrt{8\pi k_0r}}
\left[\sec\frac{\theta-\theta_0}{2}-\sec\frac{\theta+\theta_0}{2}\right]
+O(r^{-3/2}).
\end{aligned}}
$$

The first term cancels the incident [geometrical optics](../../../../../../geometrical-optics.md) field in its shadow, the second is its reflected plane wave and the last is the diffracted edge wave. The expansion is nonuniform at $\theta=\theta_0-\pi$ and $\theta=\pi-\theta_0$; the exact Fresnel expression resolves those regions. Incidence from below follows by reflecting $\theta$ and $\theta_0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
