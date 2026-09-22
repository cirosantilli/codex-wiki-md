<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [age of an FLRW universe](../../../../../../age-of-an-flrw-universe.md) at an epoch is the elapsed [cosmic time](../../../../../../cosmic-time.md) since the [Big Bang](../../../../../../big-bang.md), not the lookback time from today. For positive matter and positive [cosmological constant](../../../../../../cosmological-constant.md), integrating $dt=da/\dot a$ gives

$$
t(a)=\frac1{H_0}\int_0^a\frac{\sqrt{a'}\,da'}
{\sqrt{\Omega_{m,0}+\Omega_{\Lambda,0}a'^3}}.
$$

Put $u=\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\,a'^{3/2}$; then $du=(3/2)\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\sqrt{a'}\,da'$. The integral becomes the [age of a flat matter-Lambda universe](../../../../../../age-of-a-flat-matter-lambda-universe.md):

$$
t(a)=\frac{2}{3H_0\sqrt{\Omega_{\Lambda,0}}}
\int_0^{\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\,a^{3/2}}
\frac{du}{\sqrt{1+u^2}}
=\frac{2\operatorname{arsinh}\!\left(\sqrt{\Omega_{\Lambda,0}/\Omega_{m,0}}\,a^{3/2}\right)}
{3H_0\sqrt{\Omega_{\Lambda,0}}}.
$$

Choose $0<\theta<\pi/2$ such that $\tan\theta=\sqrt{\Omega_{m,0}/\Omega_{\Lambda,0}}\,a^{-3/2}$. The upper-limit value of $u$ is $\cot\theta$, and

$$
\operatorname{arsinh}(\cot\theta)
=\log(\cot\theta+\csc\theta)
=\log\frac{1+\cos\theta}{\sin\theta}.
$$

Consequently

$$
\boxed{t(z)=\frac{2}{3H_0\sqrt{\Omega_{\Lambda,0}}}
\log\frac{1+\cos\theta}{\sin\theta},
\qquad \tan\theta=\sqrt{\frac{\Omega_{m,0}}{\Omega_{\Lambda,0}}}(1+z)^{3/2}.}
$$

The integration constant is fixed by $t\to0$ as $z\to\infty$, where $\theta\to\pi/2$. Equivalently, differentiating $u=\cot\theta$ changes the last integral to $-\int d\theta/\sin\theta$, recovering the supplied trigonometric identity. The formula assumes positive $\Omega_{\Lambda,0}$ and $\Omega_{m,0}$; its zero-vacuum limit is regular even though this parametrization is singular.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
