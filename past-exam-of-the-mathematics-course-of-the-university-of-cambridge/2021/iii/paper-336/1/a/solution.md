<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put

$$
s=\sqrt{1-\theta^2},\qquad a=\frac1s,
\qquad
\Phi(z)=\theta\sqrt{z^2-1}-z.
$$

On the specified branch, $\sqrt{z^2-1}$ is positive for $z>1$ and negative for $z<-1$. The [saddle points](../../../../../../saddle-point.md) of the phase are therefore $z=\pm a$, with

$$
\Phi(a)=-s,\qquad \Phi(-a)=s,
$$

and

$$
\Phi''(a)=-\frac{s^3}{\theta^2},
\qquad
\Phi''(-a)=\frac{s^3}{\theta^2}.
$$

Applying the [method of steepest descent](../../../../../../method-of-steepest-descent.md) at the two simple saddles gives

$$
g_{\mathrm{sd}}\sim
\sqrt{\frac{2\pi}{\lambda}}
\frac{\theta}{s^{3/2}}
\left[
\frac{e^{i(\lambda s+\pi/4)}}{\theta a(a+z_0)}
+\frac{e^{-i(\lambda s+\pi/4)}}{\theta a(a-z_0)}
\right].
$$

This formula is valid while the pole and positive saddle remain separated by much more than their $O(\lambda^{-1/2})$ saddle width.

The pole crosses the positive saddle when

$$
z_0=a,
\qquad\text{or equivalently}\qquad
\theta=\theta_*:=\sqrt{1-z_0^{-2}}.
$$

Because the original contour passes above the pole, deformation onto the steepest-descent contour contributes

$$
g_{\mathrm p}
=-\frac{2\pi i}{\sqrt{z_0^2-1}}
\exp\left\{i\lambda
\left[\theta\sqrt{z_0^2-1}-z_0\right]\right\}
$$

when $z_0>a$, or $0<\theta<\theta_*$. It contributes no residue when $z_0<a$, or $\theta_*<\theta<1$. Hence, away from the transition,

$$
\boxed{
g\sim
\begin{cases}
g_{\mathrm{sd}}+g_{\mathrm p},&0<\theta<\theta_*,\\
g_{\mathrm{sd}},&\theta_*<\theta<1.
\end{cases}}
$$

The residue is exponentially oscillatory and $O(1)$, whereas each ordinary saddle contribution is $O(\lambda^{-1/2})$.

At $\theta=\theta_*$ the pole and saddle coalesce, so the displayed saddle formula is singular and must not be used. Passing above the coincident point gives one half of the switched residue at leading order:

$$
g\sim-\frac{\pi i}{\sqrt{z_0^2-1}}e^{-i\lambda s}.
$$

If $|\theta-\theta_*|=O(\lambda^{-1/2})$, a uniform [saddle-point approximation with a nearby pole](../../../../../../saddle-point-approximation-with-a-nearby-pole.md) replaces the discontinuous switch by a complementary-error-function multiplier.

As $\theta\to1^-$, $s\to0$, $a\to\infty$, and the pole lies in the no-residue regime. Each saddle coefficient is $O(s^{1/2}\lambda^{-1/2})$, so the leading approximation tends to

$$
\boxed{\lim_{\theta\to1^-}g(\theta;\lambda)=0}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
