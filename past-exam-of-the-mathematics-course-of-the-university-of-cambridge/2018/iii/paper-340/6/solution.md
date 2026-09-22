<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Either essay option suffices; both are developed here to make the two mathematical constructions available.

**Diffusion for images.** Model grey level as $u(x,t)$, initially $g(x)$, and use a [Neumann boundary condition](../../../../../neumann-boundary-condition.md) to avoid flux across an image boundary. The linear [heat equation](../../../../../heat-equation.md) $u_t=\Delta u$ smooths the data. On $\mathbb R^2$ its solution is [convolution](../../../../../convolution.md) with the [heat kernel](../../../../../heat-kernel.md), $G_t(x)=(4\pi t)^{-1}\exp(-|x|^2/(4t))$. Equivalently each [Fourier mode](../../../../../fourier-mode.md) is multiplied by $e^{-t|\xi|^2}$, suppressing high frequencies and noise. With no flux, the mean is conserved and

$$
\frac d{dt}\frac12\int u^2=-\int|\nabla u|^2\le0.
$$

The drawback is that sharp edges also contain high frequencies: a step becomes a transition of width comparable to $\sqrt t$. Running the [heat equation](../../../../../heat-equation.md) backwards attempts sharpening but amplifies modes by $e^{t|\xi|^2}$ and is [ill-posed](../../../../../ill-posed-problem.md).

The [Perona-Malik equation](../../../../../perona-malik-equation.md) instead uses a decreasing diffusivity,

$$
u_t=\operatorname{div}(c(|\nabla u|)\nabla u),\qquad
c(r)=\frac1{1+(r/K)^2},\quad K>0.
$$

Small gradients are smoothed strongly and large ones less strongly. If $n=\nabla u/|\nabla u|$ and $t$ is a unit tangent to a level curve, then away from zero gradient,

$$
u_t=[c(r)+rc'(r)]u_{nn}+c(r)u_{tt},\qquad r=|\nabla u|.
$$

The derivative of the flux, rather than just $c(r)>0$, controls forward parabolicity. Here $c(r)+rc'(r)=[1-(r/K)^2]/[1+(r/K)^2]^2$ becomes negative for $r>K$: smoothing remains tangential but the normal direction can sharpen. This formal edge enhancement comes with forward-backward [ill-posedness](../../../../../ill-posed-problem.md), so existence and stability of the unregularized continuum equation must not be presumed. One regularization uses $c(|\nabla(G_\varepsilon*u)|)$ as a smoothed edge detector while keeping the flux proportional to $\nabla u$. For fixed positive $\varepsilon$, the coefficient is controlled by the smoothed data; under suitable bounds it stays positive and gives a regularized forward equation. It preserves edges through reduced cross-edge transport, without the same local backward-diffusion calculation.

[Diffusion from a gradient energy](../../../../../diffusion-from-a-gradient-energy.md) connects these equations with [variational regularization](../../../../../variational-regularization.md). If $E(u)=\int\Phi(|\nabla u|)$, its formal $L^2$ [gradient flow](../../../../../gradient-flow.md) is $u_t=\operatorname{div}(\Phi'(r)\nabla u/r)$. Linear diffusion corresponds to $\Phi(r)=r^2/2$. The displayed [Perona-Malik equation](../../../../../perona-malik-equation.md) corresponds to $\Phi(r)=(K^2/2)\log(1+r^2/K^2)$, which is nonconvex in the gradient for large $r$. A convex alternative is [total variation flow](../../../../../total-variation-flow.md), with $\Phi(r)=r$, interpreted through a [subgradient](../../../../../subgradient.md) at zero gradient. Adding squared data fidelity gives the formal evolution $u_t=\operatorname{div}(\nabla u/|\nabla u|)-(u-g)$, whose equilibrium is the unique [total variation denoising](../../../../../total-variation-denoising.md) minimizer. Convex TV preserves sharp interfaces more effectively than the heat energy, but it may produce piecewise constant plateaux, known as [staircasing in total variation denoising](../../../../../staircasing-in-total-variation-denoising.md). A stopping time or fidelity weight controls the smoothing scale. **Linear diffusion is stable but blurs edges; nonlinear diffusion must balance edge selectivity with parabolicity and regularization.**

**Wavelets on an interval.** Simply restricting a whole-line [orthonormal wavelet](../../../../../orthonormal-wavelet.md) to $[0,1]$ destroys its orthogonality and generally its [vanishing moments](../../../../../vanishing-moment.md). Periodizing the basis restores orthogonality on the circle, but treats the two endpoints as neighbors. This is suitable for periodic data and can create an artificial endpoint jump for nonperiodic data.

A localized [interval-adapted wavelet basis](../../../../../interval-adapted-wavelet-basis.md) instead uses unchanged interior functions and finitely many special [boundary wavelets](../../../../../boundary-wavelet.md) at each endpoint. Start with a sufficiently regular [compact support](../../../../../compact-support.md) orthonormal [Daubechies wavelet](../../../../../daubechies-wavelet.md) of order at least $q$ and choose a coarse level at which left and right boundary supports are disjoint. At each boundary, take appropriate finite combinations of the scaling functions that meet the endpoint, restricted to the interval. Choose these combinations to reproduce [polynomials](../../../../../polynomial-split.md) of degrees $0,\ldots,q-1$, remove dependencies, and orthonormalize the finite boundary [Gram matrix](../../../../../gram-matrix.md). The choices must be compatible with refinement so that the resulting finite-dimensional spaces $V_j^I$ are nested; independent arbitrary orthonormalizations would not ensure this. Interior functions retain their whole-line filters, while the boundary functions use finite boundary refinement matrices.

For each level, choose an [orthonormal basis](../../../../../orthonormal-basis.md) of the [orthogonal complement](../../../../../orthogonal-complement.md) $W_j^I=V_{j+1}^I\ominus V_j^I$. It consists of interior wavelets and a bounded number of left and right [boundary wavelets](../../../../../boundary-wavelet.md). Since the polynomial restrictions of degree less than $q$ belong to $V_j^I$, every member of $W_j^I$ has $q$ [vanishing moments](../../../../../vanishing-moment.md). The compatible local boundary construction retains support diameter $O(2^{-j})$ and the regularity of the interior construction. Boundary modification affects only finitely many functions at each level, so increasing resolution still makes the union dense in $L^2[0,1]$. Consequently, for a fixed coarse level $J$,

$$
\boxed{L^2[0,1]=V_J^I\oplus\mathop{\bigoplus}_{j\ge J}W_j^I.}
$$

The coarse [scaling functions](../../../../../scaling-function.md) together with all these [wavelets](../../../../../wavelet.md) form an [orthonormal basis](../../../../../orthonormal-basis.md). This construction is the [Cohen-Daubechies-Vial interval wavelet construction](../../../../../cohen-daubechies-vial-interval-wavelet-construction.md). It preserves localization, polynomial cancellation and stable coefficient extraction without imposing periodic or zero boundary data. The finite boundary refinement matrices also permit a fast transform; a mere restriction followed by one unrelated [Gram-Schmidt process](../../../../../gram-schmidt-process.md) at each scale does not establish all these properties.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 340](../../paper-340-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
