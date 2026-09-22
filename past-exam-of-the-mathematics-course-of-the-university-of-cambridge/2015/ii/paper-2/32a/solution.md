<h1 id="32a/solution">Solution</h1>

↑ **Parent:** [32A](../32a.md)

Normalize the incident plane wave to unit amplitude. The scattering asymptotics are $\psi(\mathbf r)\sim e^{ikz}+f(\theta)e^{ikr}/r$; the outgoing coefficient $f$ is the [scattering amplitude](../../../../../scattering-amplitude.md). The general axisymmetric free solution for $r>0$ is

$$
\psi(r,\theta)=\sum_{\ell\geq0}\{a_\ell j_\ell(kr)+b_\ell n_\ell(kr)\}P_\ell(\cos\theta),
$$

using [Spherical Bessel functions](../../../../../spherical-bessel-function.md), [spherical Neumann functions](../../../../../spherical-bessel-function-of-the-second-kind.md) and [Legendre polynomials](../../../../../legendre-polynomial.md).

For a real short-range central potential, the exterior radial solution in each [partial wave](../../../../../partial-wave.md) is proportional to $\cos\delta_\ell\,j_\ell-\sin\delta_\ell\,n_\ell$, whose large-$r$ form is $\sin(kr-\ell\pi/2+\delta_\ell)/(kr)$. This defines the [scattering phase shift](../../../../../scattering-phase-shift.md). Multiplying this combination by $(2\ell+1)i^\ell e^{i\delta_\ell}$ matches the incoming spherical component of the incident plane wave: the factor $e^{i\delta_\ell}$ cancels the shifted incoming phase. The outgoing coefficient instead acquires $e^{2i\delta_\ell}$. Subtracting the plane wave's outgoing component therefore gives

$$
\boxed{f(\theta)=\frac1{2ik}\sum_{\ell\geq0}(2\ell+1)(e^{2i\delta_\ell}-1)P_\ell(\cos\theta)=\frac1k\sum_{\ell\geq0}(2\ell+1)e^{i\delta_\ell}\sin\delta_\ell\,P_\ell(\cos\theta).}
$$

For the barrier's $s$-wave, the regular reduced radial function inside is $u(r)=A\sinh(\kappa r)$, with $\kappa=\sqrt{\gamma^2-k^2}$. Outside take $u(r)=B\sin(kr+\delta_0)$. Continuity of $u$ and its derivative at $a$ equates logarithmic derivatives:

$$
\kappa\coth(\kappa a)=k\cot(ka+\delta_0),\qquad\boxed{\frac{\tanh(\kappa a)}{\kappa a}=\frac{\tan(ka+\delta_0)}{ka}.}
$$

Use the branch with $\delta_0\to0$ as $k\to0$. The matching equation gives $\delta_0=k(\tanh(\gamma a)/\gamma-a)+o(k)$, so the $s$-wave [scattering amplitude](../../../../../scattering-amplitude.md) tends to

$$
\boxed{f\longrightarrow\frac{\tanh(\gamma a)-\gamma a}{\gamma}.}
$$

Its negative is the [repulsive spherical barrier scattering length](../../../../../repulsive-spherical-barrier-scattering-length.md), positive for this repulsive barrier.

## ↑ Ancestors (10)

1. [32A](../32a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
