<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\rho'=\rho-\rho_0$, and take the [retarded acoustic Green function](../../../../../../retarded-acoustic-green-function.md) for $\partial_t^2-c_0^2\nabla^2$:

$$
G_R(x-y,t-\tau)=\frac{\delta(t-\tau-|x-y|/c_0)}{4\pi c_0^2|x-y|}.
$$

This selects the causal, outgoing [acoustic density perturbation](../../../../../../acoustic-density-perturbation.md), with no additional incoming homogeneous [wave equation](../../../../../../wave-equation-split.md) solution. Convolving the [acoustic dipole](../../../../../../acoustic-dipole.md) forcing with this [Green function](../../../../../../green-s-function.md) and moving its spatial [derivative](../../../../../../derivative.md) outside the integral gives

$$
\rho'=-\partial_{x_i}\int d\tau\int d^3y\,
\frac{F_i(y,\tau)\delta(f(y,\tau))|\nabla_y f(y,\tau)|}{4\pi c_0^2|x-y|}
\delta\left(t-\tau-\frac{|x-y|}{c_0}\right).
$$

The [surface delta distribution](../../../../../../surface-delta-distribution.md) converts the spatial integral to the moving surface. At fixed surface labels $(p,q)$, set

$$
r(\tau)=|x-y(p,q,\tau)|,\quad
\widehat r=\frac{x-y}{|x-y|},\quad v=\partial_\tau y(p,q,\tau),\quad
M_r=\frac{\widehat r\cdot v}{c_0}.
$$

The [radial Mach number](../../../../../../radial-mach-number.md) enters the [moving-surface retarded Jacobian](../../../../../../moving-surface-retarded-jacobian.md), because $dr/d\tau=-\widehat r\cdot v$ and hence

$$
\frac d{d\tau}\left(t-\tau-\frac{r(\tau)}{c_0}\right)=-(1-M_r).
$$

Let $\tau^*$ be a root of the [retarded time](../../../../../../retarded-time.md) equation

$$
\boxed{t=\tau^*+\frac{|x-y(p,q,\tau^*)|}{c_0}.}
$$

The delta change-of-variable rule now gives

$$
\boxed{\rho'(x,t)=-\partial_{x_i}\iint
\left[\frac{F_i(y,\tau)h_ph_q}{4\pi c_0^2|x-y|\,|1-M_r|}\right]_{\tau=\tau^*}dp\,dq.}
$$

Here $h_p h_q$ is the surface-area factor from the orthogonal surface coordinates. For a subsonic surface, $|v|<c_0$, the retarded equation is monotone in $\tau$ and has one root when the motion is defined for the required past times. For more general motion, sum the displayed contribution over all simple retarded roots. A root with $1-M_r=0$ requires a separate limiting treatment; the simple-root formula does not apply there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
