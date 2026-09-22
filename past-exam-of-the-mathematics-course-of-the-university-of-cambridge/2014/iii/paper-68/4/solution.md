<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In [diffusion image processing](../../../../../diffusion-image-processing.md), the observed grey-value [image signal](../../../../../image-signal.md) $g$ is the initial condition for an evolution $u(x,t)$; time controls the [image smoothing](../../../../../image-smoothing.md) scale. A useful model must suppress [image noise](../../../../../image-noise.md) while respecting the [image signal](../../../../../image-signal.md)'s geometric boundaries. Unless exterior values are intended, use periodic boundaries or [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), so the filter does not lose intensity through the [image signal](../../../../../image-signal.md) border.

The basic linear model is the [heat equation](../../../../../heat-equation.md), $u_t=\Delta u$, $u(0)=g$. On the whole plane,

$$
\boxed{u(\cdot,t)=G_t*g,\qquad
G_t(x)=\frac1{4\pi t}e^{-|x|^2/(4t)}.}
$$

It is Gaussian [image smoothing](../../../../../image-smoothing.md) with variance $2t$ in each coordinate. In Fourier variables, $\widehat u(\xi,t)=e^{-t|\xi|^2}\widehat g(\xi)$: high spatial frequencies are damped most strongly. Under zero-flux or periodic boundaries the mean is conserved, the maximum principle keeps values within the initial range, and

$$
\frac d{dt}\frac12\int_\Omega(u-\bar u)^2dx=-\int_\Omega|\nabla u|^2dx\leq0.
$$

These give stable [image noise](../../../../../image-noise.md) suppression, but a sharp step also contains high frequencies and is blurred across a width of order $\sqrt t$. Constant diffusivity has no mechanism for distinguishing [image noise](../../../../../image-noise.md) from an [image edge](../../../../../image-edge.md).

Linear sharpening by the backward [heat equation](../../../../../heat-equation.md) would multiply Fourier modes by $e^{t|\xi|^2}$ and amplify arbitrarily fine [image noise](../../../../../image-noise.md) without bound. It is an ill-posed initial-value problem. A controlled [unsharp masking](../../../../../unsharp-masking.md) step instead uses $g+\lambda(g-G_t*g)$, with multiplier $1+\lambda(1-e^{-t|\xi|^2})$. This amplifies high frequencies by at most $1+\lambda$; it can improve apparent contrast but also amplifies [image noise](../../../../../image-noise.md) and cannot reliably restore information already lost by [image smoothing](../../../../../image-smoothing.md).

Nonlinear models use [image signal](../../../../../image-signal.md) structure to select the diffusion. A gradient-based energy and its formal $L^2$ [gradient flow](../../../../../gradient-flow.md) are

$$
E(u)=\int_\Omega\Psi(|\nabla u|)dx+\frac\lambda2\int_\Omega(u-g)^2dx,
\qquad
u_t=\operatorname{div}\big(c(|\nabla u|)\nabla u\big)-\lambda(u-g),
\quad c(s)=\frac{\Psi'(s)}s.
$$

For a smooth solution with the corresponding zero-flux condition, $dE/dt=-\int u_t^2\leq0$. The fidelity term prevents indefinite drift towards a constant reconstruction; pure diffusion is usually stopped at a selected finite time.

The local [principal diffusion coefficients](../../../../../principal-diffusion-coefficients.md) distinguish suppression of diffusion from backward diffusion. Where $s=|\nabla u|>0$, the flux [derivative](../../../../../derivative.md) is

$$
c(s)I+\frac{c'(s)}s\nabla u\otimes\nabla u.
$$

Its coefficient along an [image signal](../../../../../image-signal.md) level curve is $c(s)$; across that curve it is $c(s)+sc'(s)=\Psi''(s)$. Forward parabolic behavior requires both coefficients nonnegative, with strict positive lower bounds giving uniform parabolicity. Merely choosing $c>0$ and decreasing does not establish well-posedness.

For a convex area-type penalty $\Psi(s)=\sqrt{\varepsilon^2+s^2}$, the coefficients are

$$
c(s)=\frac1{\sqrt{\varepsilon^2+s^2}},\qquad
c(s)+sc'(s)=\frac{\varepsilon^2}{(\varepsilon^2+s^2)^{3/2}}>0.
$$

Diffusion across steep [image edges](../../../../../image-edge.md) is weak but remains forward. As $\varepsilon\to0$, the [total variation flow](../../../../../total-variation-flow.md) formally becomes $u_t=\operatorname{div}(\nabla u/|\nabla u|)$. Its convex [subgradient](../../../../../subgradient.md) formulation handles flat regions and discontinuities. It favors piecewise constant [image signals](../../../../../image-signal.md) and preserves sharp transitions better than Gaussian [image smoothing](../../../../../image-smoothing.md), but can produce [staircasing in total variation denoising](../../../../../staircasing-in-total-variation-denoising.md), shrink small objects and move boundaries by [curvature](../../../../../curvature.md). [image edge](../../../../../image-edge.md) preservation does not mean exact preservation of all [image edge](../../../../../image-edge.md) locations or amplitudes.

The [Perona-Malik equation](../../../../../perona-malik-equation.md) takes a decreasing diffusivity such as $c(s)=1/(1+s^2/\kappa^2)$. Small [gradients](../../../../../gradient.md) are smoothed strongly, while large [gradients](../../../../../gradient.md) have weak flux. More precisely,

$$
\boxed{c(s)+sc'(s)=\frac{1-s^2/\kappa^2}{(1+s^2/\kappa^2)^2}.}
$$

For $s>\kappa$, diffusion in the [gradient](../../../../../gradient.md) direction is backward, so a strong transition can steepen. This gives formal [image edge](../../../../../image-edge.md) enhancement but also causes instability and continuum [ill-posedness](../../../../../ill-posed-problem.md). The exponential choice $c(s)=e^{-s^2/\kappa^2}$ similarly has a negative normal coefficient for $s>\kappa/\sqrt2$. Discrete results depend on the stencil, step size and implicit regularization; appealing visual results are not a proof of a well-posed PDE.

A [regularized Perona-Malik diffusion](../../../../../regularized-perona-malik-diffusion.md) computes the conductance from a smoothed [image signal](../../../../../image-signal.md), for example

$$
u_t=\operatorname{div}\big(c(|\nabla(G_\sigma*u)|)\nabla u\big).
$$

The flux still acts on $u$, but the [image edge](../../../../../image-edge.md) detector is less sensitive to raw [image noise](../../../../../image-noise.md). With a smooth kernel and a positive conductance bounded away from zero on the attained range, the local principal diffusion is forward; appropriate regularity and boundary assumptions give a well-posed nonlocal parabolic model. The exact regularization and fixed [image smoothing](../../../../../image-smoothing.md) scale are part of the model.

A genuinely directional filter uses a [diffusion tensor for image filtering](../../../../../diffusion-tensor-for-image-filtering.md):

$$
u_t=\operatorname{div}(D\nabla u),\qquad
D=a_n e_ne_n^T+a_t e_te_t^T,\quad 0<a_n\ll a_t.
$$

Here $e_n$ estimates the [image edge](../../../../../image-edge.md) normal and $e_t$ its tangent. A [structure tensor](../../../../../structure-tensor.md) $J_\rho=G_\rho*(\nabla u_\sigma\nabla u_\sigma^T)$ provides robust directions at a second averaging scale. Strong tangent diffusion smooths [image noise](../../../../../image-noise.md) along an [image edge](../../../../../image-edge.md), while weak normal diffusion reduces mixing across it. Related coherence-enhancing choices connect elongated features along their dominant orientation. Positive tensor [eigenvalues](../../../../../eigenvalue.md) preserve forward parabolicity; this type of enhancement must be distinguished from Perona–Malik's backward normal diffusion.

For more direct sharpening, a [shock filter for image enhancement](../../../../../shock-filter-for-image-enhancement.md) formally evolves $u_t=-\operatorname{sign}(\Delta u)|\nabla u|$. It is a Hamilton–Jacobi-type transport mechanism, not a positive diffusion operator, and steepens transitions around inflection boundaries. In practice it can be combined with regularized forward diffusion to control [image noise](../../../../../image-noise.md). Any enhancement method needs a scale or stopping rule and an honest treatment of [image noise](../../../../../image-noise.md) amplification.

**Linear heat flow offers predictable [image smoothing](../../../../../image-smoothing.md) but blurs [image edges](../../../../../image-edge.md); convex nonlinear diffusion can preserve them; backward or shock mechanisms sharpen them at a greater stability cost.** [Gradient](../../../../../gradient.md) thresholds, conductance regularization and positive tensor directions determine which of these behaviors a proposed filter actually has.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
