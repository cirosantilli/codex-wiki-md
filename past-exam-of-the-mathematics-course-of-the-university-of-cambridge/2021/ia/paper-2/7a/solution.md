<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Put $\omega=\dot\theta$. The first-order system is

$$
\boxed{
\dot\theta=\omega,\qquad
\dot\omega=-\sin\theta
\left(\lambda-2\mu+\frac{2\mu}{\sqrt{5+4\cos\theta}}\right)}.
$$

Write

$$
h(\theta)=\lambda-2\mu
+\frac{2\mu}{\sqrt{5+4\cos\theta}}.
$$

On $[0,\pi]$, $h$ is strictly increasing. Moreover,

$$
h(0)=\lambda-\frac{4\mu}{3}<0,
\qquad
h(\pi)=\lambda>0
$$

when $3\lambda<4\mu$. Thus there is one $\theta_*\in(0,\pi)$ with $h(\theta_*)=0$, in addition to the fixed points at $\theta=0,\pi$. Explicitly,

$$
\boxed{
\cos\theta_*
=\frac{\mu^2}{(2\mu-\lambda)^2}-\frac54}.
$$

Let $g(\theta)=\sin\theta\,h(\theta)$. Linearization at $(\theta_0,0)$ has eigenvalues satisfying

$$
\sigma^2=-g'(\theta_0).
$$

At zero, $g'(0)=h(0)<0$, and at $\pi$, $g'(\pi)=-h(\pi)<0$, so both endpoints are saddles. At the interior point,

$$
g'(\theta_*)=\sin\theta_*h'(\theta_*)>0,
$$

so $(\theta_*,0)$ is a center. On the full angular interval there is a second center at $(-\theta_*,0)$.

The system has the conserved energy of a [conservative planar phase portrait](../../../../../conservative-planar-phase-portrait.md),

$$
\boxed{
E=\frac{\omega^2}{2}
-(\lambda-2\mu)\cos\theta
-\mu\sqrt{5+4\cos\theta}}.
$$

For $\lambda=1$, $\mu=3/2$,

$$
\cos\theta_*=-\frac{11}{16}.
$$

The phase portrait on the cylinder consists of centers at $\theta=\pm\arccos(-11/16)$ surrounded by closed periodic-energy curves, with saddles at $\theta=0$ and the identified point $\theta=\pi=-\pi$. The saddle-energy contours form the separatrices between librations in the potential wells and trajectories crossing the lower barrier.

If $3\lambda>4\mu$, then $h(0)>0$ and monotonicity gives no interior zero on $(0,\pi)$. The point $(0,0)$ becomes a center, while $(\pi,0)$ remains a saddle. At $3\lambda=4\mu$, the two off-axis centers coalesce with the origin and the linearization there is degenerate.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
