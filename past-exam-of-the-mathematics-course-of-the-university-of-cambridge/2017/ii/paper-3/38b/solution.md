<h1 id="38b/solution">Solution</h1>

↑ **Parent:** [38B](../38b.md)

For the rapidly varying [wave phase](../../../../../phase-waves.md), define $k_i=\partial_i\theta$ and $\omega=-\partial_t\theta$, with the common scaling by $\varepsilon$ absorbed into these local variables. A packet moves with [group velocity](../../../../../group-velocity.md) $c_{g,i}=\partial\Omega/\partial k_i$. Along that trajectory, $d/dt=\partial_t+c_g\cdot\nabla_x$. Compatibility gives $\partial_tk_i=-\partial_i\omega$ and $\partial_i k_j=\partial_j k_i$. Differentiating the local [dispersion relation](../../../../../dispersion-relation.md) then cancels its implicit $k$ [derivatives](../../../../../derivative.md), yielding

$$
\boxed{\dot x_i=\Omega_{k_i},\quad\dot k_i=-\Omega_{x_i},\quad\dot\omega=\Omega_t.}
$$

The last equality follows also by differentiating $\omega=\Omega(k,x,t)$ along the ray and cancelling the two [Hamiltonian](../../../../../hamiltonian.md) cross terms. The partial [derivatives](../../../../../derivative.md) of $\Omega$ hold its other arguments fixed.

A mean flow adds the [Doppler shift](../../../../../doppler-effect.md): the [intrinsic frequency](../../../../../intrinsic-frequency.md) is $\widehat\omega=\omega-kU(z)$, so

$$
 (\omega-kU)^2=\frac{N^2k^2}{k^2+m^2},\qquad
 \Omega=kU+\frac{Nk}{\sqrt{k^2+m^2}}
$$

on the positive-intrinsic-frequency branch launched here. The medium is stationary and independent of $x$, so $\omega$ and $k$ are constant. Initially $m=0,U=0$, hence $\omega=N$. Moreover $\dot m=-kU'<0$, and then $\dot z=-Nkm/(k^2+m^2)^{3/2}>0$. The initial vertical [group velocity](../../../../../group-velocity.md) is zero, but $m$ immediately becomes negative and the ray accelerates upwards.

If $U$ reaches $N/k$ at a finite height $z_c$, this is the [critical level of an internal gravity wave](../../../../../critical-level-of-an-internal-gravity-wave.md), with $U(z_c)=\omega/k$. Below it,

$$
\boxed{m=-k\sqrt{\frac{N^2}{(N-kU)^2}-1}.}
$$

Assuming $0<U'(z_c)<\infty$, put $\delta=z_c-z$. Then $N-kU\sim kU'(z_c)\delta$, giving

$$
\boxed{m\sim-\frac{N}{U'(z_c)\delta},\quad
 \dot z\sim\frac{kU'(z_c)^2}{N}\delta^2,\quad
 t\sim\frac{N}{kU'(z_c)^2\delta}\longrightarrow\infty.}
$$

Thus the ray cannot cross this level in finite time within the geometrical-optics approximation. The hypothesis $U'>0,U(0)=0$ alone does not guarantee a finite $z_c$: for example $U(z)=\frac{N}{2k}(1-e^{-z})$ on $z\geq0$ never reaches $N/k$. **Existence of a finite critical level is an additional assumption**. Very close to one, diverging [wavenumber](../../../../../wavenumber.md) can invalidate the inviscid, linear, slowly varying approximation; the result is the formal ray prediction.

## ↑ Ancestors (10)

1. [38B](../38b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
