<h1 id="30a/solution">Solution</h1>

↑ **Parent:** [30A](../30a.md)

A [fundamental solution](../../../../../fundamental-solution-of-a-linear-differential-operator.md) of a constant-coefficient operator $P(D)$ is a [distribution](../../../../../distribution-mathematical-analysis.md) $E$ satisfying $P(D)E=\delta_0$. The proposed $N$ is [locally integrable](../../../../../locally-integrable-function.md) in three dimensions and harmonic away from zero. For a smooth [compactly supported](../../../../../compact-support.md) [test function](../../../../../test-function.md) $\varphi$, apply Green's identity outside the ball of radius $\eta$. On the inner boundary the outward normal is $-\hat r$, so $\partial_\nu N=1/(4\pi\eta^2)$. The outer boundary contributes nothing. Thus

$$
\int_{|x|>\eta}N(-\Delta\varphi)\,dx=\int_{|x|=\eta}\left(\frac{\varphi}{4\pi\eta^2}+\frac{\partial_r\varphi}{4\pi\eta}\right)dS.
$$

The first term tends to $\varphi(0)$ and the second is $O(\eta)$. [Local integrability](../../../../../locally-integrable-function.md) permits taking the limit on the left. Therefore **$-\Delta N=\delta_0$ in [distributions](../../../../../distribution-mathematical-analysis.md)**.

For a [harmonic function](../../../../../harmonic-function.md) on a ball, define its [spherical mean](../../../../../spherical-mean.md) $M(r)=(4\pi)^{-1}\int_{S^2}u(x_0+r\omega)\,d\omega$. Differentiation and the [divergence theorem](../../../../../divergence-theorem.md) give $M'(r)=(4\pi r^2)^{-1}\int_{B_r(x_0)}\Delta u=0$. Its limit at zero is $u(x_0)$, so

$$
\boxed{u(x_0)=\frac1{4\pi r^2}\int_{\partial B_r(x_0)}u\,dS=\frac1{|B_r|}\int_{B_r(x_0)}u\,dx.}
$$

The ball formula follows by integrating [spherical means](../../../../../spherical-mean.md) in the radius. If two solutions of the prescribed [Poisson equation](../../../../../poisson-equation.md) tend to zero at infinity, their difference is globally harmonic and also tends to zero. Apply the [spherical mean](../../../../../spherical-mean.md) at an arbitrary $x_0$ and let $r\to\infty$; every point of that sphere has distance at least $r-|x_0|$ from the origin, so the mean tends to zero. Hence the difference is zero everywhere, proving **uniqueness**.

## ↑ Ancestors (10)

1. [30A](../30a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
