<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the given harmonic potentials, $\nabla^2(\boldsymbol\Phi\cdot\mathbf x)=2\nabla\cdot\boldsymbol\Phi$. Taking the [divergence](../../../../../divergence.md) of the velocity representation therefore gives $\nabla\cdot\mathbf u=0$. Taking its [Laplacian](../../../../../laplacian.md) gives $\nabla^2\mathbf u=-2\nabla(\nabla\cdot\boldsymbol\Phi)$, so the [Stokes equations](../../../../../stokes-equation.md) hold with

$$
\boxed{p=-2\mu\nabla\cdot\boldsymbol\Phi+p_\infty.}
$$

This is the [Papkovich–Neuber representation](../../../../../papkovich-neuber-representation.md) in the sign and normalization of this problem. The potentials used in other conventions can differ by an overall factor and sign; the [velocity](../../../../../velocity.md) and [pressure](../../../../../pressure.md) must be scaled together.

**(a) Point force.** Put the singularity at the origin, $r=|\mathbf x|$, and choose $\boldsymbol\Phi=\mathbf F/(8\pi\mu r)$, $\chi=0$. The resulting [Stokeslet](../../../../../stokeslet.md) is

$$
\boxed{\mathbf u=\frac1{8\pi\mu}\left(\frac{\mathbf F}{r}+\frac{(\mathbf F\cdot\mathbf x)\mathbf x}{r^3}\right),\qquad
p-p_\infty=\frac{\mathbf F\cdot\mathbf x}{4\pi r^3}.}
$$

The harmonic calculation applies away from the force. Distributionally this is the [Green function](../../../../../green-s-function.md) for $-\nabla p+\mu\nabla^2\mathbf u+\mathbf F\delta^{(3)}(\mathbf x)=0$, with zero [divergence](../../../../../divergence.md).

**(b) Point source.** Set $\boldsymbol\Phi=0$, $\chi=-Q/(4\pi r)$. The [three-dimensional point source](../../../../../three-dimensional-point-source.md) field is

$$
\boxed{\mathbf u=\frac{Q\mathbf x}{4\pi r^3},\qquad p=p_\infty.}
$$

Its outward [volume flux](../../../../../volumetric-flow-rate.md) across every enclosing [sphere](../../../../../sphere.md) is $Q$. The [divergence](../../../../../divergence.md) is zero away from the source and equals $Q\delta^{(3)}(\mathbf x)$ distributionally, so the singular point represents volume injection rather than an incompressible material point.

**(c) Stresslet.** Let $G_{ij}(\mathbf x)=(\delta_{ij}/r+x_ix_j/r^3)/(8\pi\mu)$ and use a symmetric trace-free [stresslet tensor](../../../../../particle-stresslet-tensor.md) $S$ with the convention $u_i=-S_{jk}\partial_kG_{ij}$. Differentiating the [Stokeslet](../../../../../stokeslet.md) and using symmetry and zero trace gives

$$
\boxed{u_i=\frac{3x_i(\mathbf x\cdot S\mathbf x)}{8\pi\mu r^5},\qquad
p-p_\infty=\frac{3\mathbf x\cdot S\mathbf x}{4\pi r^5}.}
$$

For an axial [force-dipole flow](../../../../../force-dipole-flow.md) with axis $\mathbf n$, write $S=s(\mathbf n\mathbf n-I/3)$. Then the radial factor is proportional to $s[3(\mathbf n\cdot\widehat{\mathbf x})^2-1]$. Specifying the derivative convention is essential for interpreting the signs of image strengths.

**(d) Source dipole.** A positive source and negative source separated by a vector $\boldsymbol\ell$ have moment $\mathbf M=Q\boldsymbol\ell$. Their dipole limit is minus the directional derivative of the unit source field. Hence the [source dipole](../../../../../source-dipole.md) has

$$
\boxed{\mathbf u=\frac1{4\pi}\left[\frac{3(\mathbf M\cdot\mathbf x)\mathbf x}{r^5}-\frac{\mathbf M}{r^3}\right],\qquad
\chi=-\frac{\mathbf M\cdot\mathbf x}{4\pi r^3},\qquad p=p_\infty.}
$$

It carries no net [volume flux](../../../../../volumetric-flow-rate.md), and unlike a [stresslet](../../../../../force-dipole-flow.md) it is an irrotational [potential flow](../../../../../potential-flow.md).

Now set $\mathbf r=\mathbf x-d\mathbf n$ and $\mathbf R=\mathbf x+d\mathbf n$, with $d>0$. Define the unscaled kernels $K(\mathbf R)=\mathbf n/R+(\mathbf n\cdot\mathbf R)\mathbf R/R^3$, $H(\mathbf R)=\mathbf R/R^3$, and let $\partial_n=\mathbf n\cdot\nabla_{\mathbf R}$. The [no-slip image system of a normal Stokeslet](../../../../../no-slip-image-system-of-a-normal-stokeslet.md) is

$$
\boxed{\mathbf u=\frac{F}{8\pi\mu}\{K(\mathbf r)-K(\mathbf R)+2d\partial_nK(\mathbf R)-2d^2\partial_nH(\mathbf R)\}.}
$$

The reflected [Stokeslet](../../../../../stokeslet.md) has force $-F\mathbf n$. With the conventions above, the remaining image strengths are

$$
\boxed{S=-2Fd(\mathbf n\mathbf n-I/3),\qquad \mathbf M=\frac{Fd^2}{\mu}\mathbf n.}
$$

The isotropic part of $S$ produces zero [velocity](../../../../../velocity.md), because $\partial_jG_{ij}=0$. Its inclusion simply puts the tensor in standard trace-free form. The [pressure](../../../../../pressure.md) follows by superposition:

$$
p-p_\infty=\frac F{4\pi}\left[\frac{\mathbf n\cdot\mathbf r}{r^3}-\frac{\mathbf n\cdot\mathbf R}{R^3}+2d\left(\frac1{R^3}-\frac{3(\mathbf n\cdot\mathbf R)^2}{R^5}\right)\right].
$$

To verify the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) explicitly, write $\mathbf x=\boldsymbol\rho$ on the plane, with $\boldsymbol\rho\cdot\mathbf n=0$, and let $b^2=\rho^2+d^2$. Then

$$
\begin{aligned}
K(\mathbf r)-K(\mathbf R)&=-2d\boldsymbol\rho/b^3,\\
\partial_nK(\mathbf R)&=\mathbf R(1/b^3-3d^2/b^5),\\
\partial_nH(\mathbf R)&=\mathbf n/b^3-3d\mathbf R/b^5.
\end{aligned}
$$

The $b^{-5}$ terms cancel, while the remaining image contribution is $2d(\mathbf R-d\mathbf n)/b^3=2d\boldsymbol\rho/b^3$. Thus both normal and tangential [velocity](../../../../../velocity.md) vanish. All image singularities lie outside the fluid, so the physical half-space contains only the prescribed force.

For the far field, expand about the wall origin. The pair of opposite forces starts with $-2d\partial_nK$; the image [stresslet](../../../../../force-dipole-flow.md) cancels this entire $r^{-2}$ term. The first surviving field is

$$
\mathbf u\sim\frac{Fd^2}{4\pi\mu}(\partial_n^2K-\partial_nH).
$$

Writing $z=\mathbf x\cdot\mathbf n$ and now $r=|\mathbf x|$, this is

$$
\mathbf u\sim\frac{3Fd^2}{4\pi\mu}\left[-\frac{2z\mathbf x}{r^5}-\frac{z^2\mathbf n}{r^5}+\frac{5z^3\mathbf x}{r^7}\right].
$$

Therefore **the generic fixed-angle far-field velocity decays as $r^{-3}$**, rather than the $r^{-1}$ free-space [Stokeslet](../../../../../stokeslet.md) or an uncancelled $r^{-2}$ [stresslet](../../../../../force-dipole-flow.md). Along the wall it is exactly zero; at fixed height and large horizontal distance the leading tangential field instead scales as $\rho^{-4}$, consistent with the angular zeros of the displayed far field.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
