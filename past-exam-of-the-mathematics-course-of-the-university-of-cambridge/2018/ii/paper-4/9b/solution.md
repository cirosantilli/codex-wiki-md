<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

For small $\theta$,

$$
1-\cos\theta=\frac{\theta^2}{2}\left(1-\frac{\theta^2}{12}+O(\theta^4)\right),
\qquad
\theta-\sin\theta=\frac{\theta^3}{6}\left(1-\frac{\theta^2}{20}+O(\theta^4)\right).
$$

Put $u=(6t/B)^{1/3}$. Inverting the second series gives

$$
\theta=u\left(1+\frac{u^2}{60}+O(u^4)\right).
$$

Substitution into the first series yields

$$
R=\frac{AR_0}{2}\left(\frac{6t}{B}\right)^{2/3}
\left[1-\frac1{20}\left(\frac{6t}{B}\right)^{2/3}+O(t^{4/3})\right].
$$

Using the definitions of $A$ and $B$ simplifies its leading factor to

$$
\frac A2\left(\frac6B\right)^{2/3}t^{2/3}
=\Omega_{m,0}^{1/3}\left(\frac{3H_0t}{2}\right)^{2/3}
=\Omega_{m,0}^{1/3}a(t).
$$

Therefore

$$
\boxed{R(t)=R_0\Omega_{m,0}^{1/3}a(t)
\left[1-\frac1{20}\left(\frac{6t}{B}\right)^{2/3}+O(t^{4/3})\right].}
$$

The homogeneous sphere containing the same mass has radius $\bar R=R_0\Omega_{m,0}^{1/3}a(t)$. By mass conservation, its nonlinear [density contrast](../../../../../density-contrast.md) is

$$
1+\delta=\left(\frac{\bar R}{R}\right)^3
=1+\frac3{20}\left(\frac{6t}{B}\right)^{2/3}+O(t^{4/3}).
$$

The leading, [linear cosmological density perturbation](../../../../../linear-cosmological-density-perturbation-split.md) is consequently

$$
\boxed{\delta_{\rm linear}(t)=\frac3{20}\left(\frac{6t}{B}\right)^{2/3}\propto t^{2/3}\propto a(t).}
$$

In the parametric solution, complete spherical collapse occurs at $\theta=2\pi$, when $R=0$ and $t=B(2\pi-\sin2\pi)=2\pi B$. Extrapolating the linear growing mode to that time gives the standard [linear spherical-collapse threshold](../../../../../linear-spherical-collapse-threshold.md)

$$
\boxed{\delta_{\rm linear,coll}
=\frac3{20}(12\pi)^{2/3}\simeq1.686.}
$$

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
