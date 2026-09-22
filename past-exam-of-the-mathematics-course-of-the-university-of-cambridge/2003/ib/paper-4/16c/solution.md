<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

[Irrotational flow](../../../../../irrotational-flow.md) means $\nabla\times\boldsymbol u=0$; [incompressible flow](../../../../../incompressible-flow.md) means $\nabla\cdot\boldsymbol u=0$. The given [streamfunction](../../../../../stream-function.md) automatically satisfies the second condition, since $\partial_x\psi_y-\partial_y\psi_x=0$. For an oriented path with unit tangent $(dx/ds,dy/ds)$, choose its right-hand unit normal $\boldsymbol n=(dy/ds,-dx/ds)$. Then

$$
\boldsymbol u\cdot\boldsymbol n\,ds=\psi_y\,dy+\psi_x\,dx=d\psi,
\qquad
\boxed{\int_{\boldsymbol x_1}^{\boldsymbol x_2}\boldsymbol u\cdot\boldsymbol n\,ds
=\psi(\boldsymbol x_2)-\psi(\boldsymbol x_1)}.
$$

The opposite normal reverses the sign; the source's unspecified normal orientation must be chosen consistently. The [volume flux](../../../../../volumetric-flow-rate.md) between two [streamlines](../../../../../streamline.md) is thus their [streamfunction](../../../../../stream-function.md) difference. A closed [contour](../../../../../complex-integration-contour.md) has zero net flux, expressing [mass conservation](../../../../../mass-conservation.md) for constant-density flow without a source inside.

For the channel, a rigid boundary has zero normal velocity and hence constant [streamfunction](../../../../../stream-function.md). Choose zero on the lower wall. Uniform inflow at infinity must have horizontal velocity $-m$, so there $\psi=-my$. The upper wall then has constant $-m$. The unbroken left wall connects to it and also has constant $-m$. The jump by $m$ between the walls at the corner represents the withdrawn flux. Finally the vorticity is $v_x-u_y=-\Delta\psi$, so irrotationality gives $\Delta\psi=0$.

Write $\psi=-my+w$. Then $w$ vanishes at $y=0,1$ and at infinity, while $w(0,y)=-m(1-y)$ for $0<y<1$. [Separation of variables](../../../../../separation-of-variables.md) gives the [harmonic sine mode in a half-strip](../../../../../harmonic-sine-mode-in-a-half-strip.md) $e^{-n\pi x}\sin n\pi y$. The [Fourier sine series](../../../../../fourier-sine-series.md) coefficients of the left boundary are

$$
b_n=2\int_0^1[-m(1-y)]\sin(n\pi y)\,dy=-\frac{2m}{n\pi}.
$$

Therefore the [corner sink in a semi-infinite channel](../../../../../corner-sink-in-a-semi-infinite-channel.md) is

$$
\boxed{\psi(x,y)=-my-\frac{2m}{\pi}\sum_{n=1}^\infty\frac{e^{-n\pi x}\sin(n\pi y)}n}.
$$

For $x>0$ the series and its differentiated series converge on compact subsets, making the sum harmonic. At $x=0$, $\sum_{n\ge1}\sin(n\pi y)/n=\pi(1-y)/2$ for $0<y<1$, so the left-wall value is exactly $-m$. The other wall values and far-field limit follow directly.

**The plus sign printed in the final series is inconsistent with the printed [boundary conditions](../../../../../boundary-condition.md).** It would give $m-2my$ on the left wall, not $-m$. The negative sign above is required. As a local flux check, near the corner the wall values give $\psi\sim-2m\theta/\pi$; the radial velocity is $-2m/(\pi r)$ and its outward flux across a quarter-circle is $-m$, precisely withdrawal.

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
