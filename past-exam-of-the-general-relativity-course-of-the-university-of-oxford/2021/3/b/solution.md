<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mu=GM/c^2$, $f=1-2\mu/r$, $q=\sqrt{1-3\mu/r}=1/u^0$, and choose $\Omega>0$. A torque-free test [gyroscope](../../../../gyroscope.md) moving on a [geodesic](../../../../geodesic.md) has a [spin four-vector](../../../../spin-four-vector.md) obeying [parallel transport](../../../../parallel-transport.md),

$$
\frac{ds^\mu}{dt}+\Gamma^\mu_{\alpha\beta}\frac{dx^\alpha}{dt}s^\beta=0,
\qquad g_{\mu\nu}u^\mu s^\nu=0.
$$

The orthogonality condition says the temporal spin component vanishes in the body's [rest frame](../../../../rest-frame.md), not necessarily in Schwarzschild coordinates. Here it gives

$$
s^t=\frac{r^2\Omega}{fc^2}s^\phi.
$$

In addition to the radial [Christoffel symbols](../../../../christoffel-symbol.md) in part (a), use $\Gamma^t_{tr}=\mu/(r^2f)$ and $\Gamma^\phi_{r\phi}=1/r$. On the equator the [parallel transport](../../../../parallel-transport.md) equations become

$$
\frac{ds^t}{dt}=-\frac{\mu}{r^2f}s^r,\qquad
\frac{ds^r}{dt}=r\Omega q^2s^\phi,\qquad
\frac{ds^\phi}{dt}=-\frac{\Omega}{r}s^r,\qquad
\frac{ds^\theta}{dt}=0.
$$

The radial equation follows by substituting $s^t$ into $ds^r/dt+\Gamma^r_{tt}s^t+\Omega\Gamma^r_{\phi\phi}s^\phi=0$. Eliminating $s^\phi$ gives $d^2s^r/dt^2+\Omega^2q^2s^r=0$.

Let $s_0$ be the invariant spin magnitude. Initially radial spin means $s^r(0)=s_0\sqrt f$ and $s^t(0)=s^\phi(0)=s^\theta(0)=0$. The complete solution is

$$
\boxed{\begin{aligned}
s^r(t)&=s_0\sqrt f\cos(\Omega qt),\\
s^\phi(t)&=-\frac{s_0\sqrt f}{rq}\sin(\Omega qt),\\
s^\theta(t)&=0,\\
s^t(t)&=-\frac{s_0r\Omega}{c^2\sqrt f\,q}\sin(\Omega qt).
\end{aligned}}
$$

To interpret the orientation, convert coordinate components into the orbiting [orthonormal frame](../../../../orthonormal-frame-in-spacetime.md). The [Lorentz factor](../../../../lorentz-factor.md) relative to a [Schwarzschild static observer](../../../../schwarzschild-static-observer.md) is $\gamma=\sqrt f/q$, so the body's measured radial and tangential spin components are

$$
S^{\hat r}=\frac{s^r}{\sqrt f}=s_0\cos(\Omega qt),\qquad
S^{\hat\phi}=\frac{rs^\phi}{\gamma}=-s_0\sin(\Omega qt).
$$

Their squared sum is $s_0^2$, and their angle relative to the outward radial direction decreases uniformly at rate

$$
\boxed{\Omega_r=\Omega q=\frac{\Omega}{u^0}.}
$$

The differing coordinate amplitudes in $s^r,s^\phi$ must not be interpreted as a nonuniform physical spin rotation. After one orbital period the radial basis has turned by $2\pi$ while the spin has turned by $-2\pi q$ relative to it. The residual [geodetic precession](../../../../geodetic-effect.md) is $\Delta\psi=2\pi(1-q)$ in the orbital direction.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
