<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) the [saddle-focus](../../../../../../saddle-focus-equilibrium.md) [linearization](../../../../../../linearization.md) is

$$
\dot r=\lambda_-r,\qquad \dot\theta=\omega,\qquad \dot z=\lambda_+z.
$$

Use a small incoming neighborhood of the stated section point $(\rho,0,-\mu)$. A nearby incoming cylinder $r=\rho$ is smoothly equivalent to that section for this calculation. Denote the positive unstable passage coordinate by $x=z_{\rm in}>0$ and leave at $z=h$. Then

$$
T=\lambda_+^{-1}\log(h/x),\qquad
r_{\rm out}=r_{\rm in}(x/h)^\delta,\qquad
\theta_{\rm out}=\theta_{\rm in}+\frac{\omega}{\lambda_+}\log(h/x).
$$

The global map is smooth in the outgoing Cartesian coordinates $r_{\rm out}\cos\theta_{\rm out}$ and $r_{\rm out}\sin\theta_{\rm out}$. Its returned unstable coordinate therefore has the leading form

$$
z_{\rm new}=-\mu+c_1r_{\rm out}\cos\theta_{\rm out}+c_2r_{\rm out}\sin\theta_{\rm out}+O(r_{\rm out}^2).
$$

Combining the two trigonometric terms, absorbing the fixed scales into the [amplitude](../../../../../../wave-amplitude.md) and phase, and using the evenness of cosine gives

$$
\boxed{x_{\rm new}=f_S(x)=-\mu+Ax^\delta\cos(q\log x+\Phi),\qquad q=\omega/\lambda_+.}
$$

The returned radial section coordinate is $\rho+O(x^\delta)$, supplying the thin transverse direction of the full two-dimensional return. In particular its [determinant](../../../../../../determinant.md) has order $x^{2\delta-1}$; the exponent is also obtained by integrating the [flow](../../../../../../flow.md) divergence $\lambda_++2\lambda_-$ over the local flight. Thus $\delta>1/2$ is the volume-contracting range. Corrections from the returned radial deviation enter at order $x^{2\delta}$, smaller than the fixed-point term $x$ in this range. Only positive returned $x$ on the chosen branch belong to the scalar return domain.

For $\delta>1$,

$$
f'_S(x)=Ax^{\delta-1}[\delta\cos(q\log x+\Phi)-q\sin(q\log x+\Phi)]\longrightarrow0.
$$

For small $\mu<0$, there is one small attracting [fixed point](../../../../../../fixed-point.md) $x=-\mu+O(|\mu|^\delta)$, representing a stable long-period [periodic orbit](../../../../../../periodic-orbit.md). It ends in the homoclinic connection at $\mu=0$; for $\mu>0$ there is no sufficiently small positive [fixed point](../../../../../../fixed-point.md). The oscillations alone do not create expanding chaos when their [derivative](../../../../../../derivative.md) tends to zero.

For $1/2<\delta<1$, there is both net volume [contraction](../../../../../../contraction-mapping.md) and a positive [saddle equilibrium](../../../../../../saddle-equilibrium.md) value $\lambda_++\lambda_->0$. At the connection, [fixed points](../../../../../../fixed-point.md) satisfy

$$
\cos(q\log x+\Phi)=\frac{x^{1-\delta}}A.
$$

The right side tends to zero, while the phase runs through infinitely many rotations. There are therefore infinitely many positive [fixed points](../../../../../../fixed-point.md) accumulating at zero near successive cosine zeros. Their successive size ratios tend to $e^{-\pi/q}$ and their [derivative](../../../../../../derivative.md) magnitudes diverge. In the full return they are [saddle equilibrium](../../../../../../saddle-equilibrium.md) [periodic orbits](../../../../../../periodic-orbit.md): one multiplier expands and the thin transverse direction contracts. Their [flow](../../../../../../flow.md) periods grow as $\lambda_+^{-1}\log(h/x)$.

The oscillatory graph also supplies the complicated itineraries. Take a sufficiently small positive return interval. Near successive zero crossings, narrow monotone subintervals map across that interval with arbitrarily large slope. Two or more inverse branches contract into it, so repeated inverse choices give symbolic invariant sets just as in part (a); lifting the strips to the thin two-dimensional return gives horseshoes and infinitely many [periodic orbits](../../../../../../periodic-orbit.md). This explains the Shilnikov chaotic mechanism rather than only naming it.

For nonzero splitting, the graph shifts vertically. Fixed-point tangencies with slope $+1$ create [saddle-node bifurcations](../../../../../../saddle-node-bifurcation.md) of [periodic orbits](../../../../../../periodic-orbit.md); crossings of slope $-1$ give period doubling. Near an oscillatory extremum the [derivative](../../../../../../derivative.md) can be small, allowing stable periodic windows. Such thresholds accumulate geometrically toward the homoclinic parameter, interspersed with expanding returns. Hence the unfolding can contain complicated switching, arbitrarily long periods and chaos, rather than a single attracting periodic branch. This is [log-periodic accumulation of Shilnikov cycles](../../../../../../log-periodic-accumulation-of-shilnikov-cycles.md). The conclusion concerns invariant sets and possible attractors allowed by the return geometry; it does not assert that a homoclinic connection alone makes all nearby trajectories chaotic.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
