<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the static nonrotating source, use [spherical symmetry](../../../../../spherical-symmetry.md) and the [static scalar perturbation of Minkowski spacetime](../../../../../static-scalar-perturbation-of-minkowski-spacetime.md), with isotropic radius $\rho$:

$$
ds^2=(1+2A)dt^2-(1+2C)(d\rho^2+\rho^2d\Omega^2).
$$

To first order, the [Einstein tensor](../../../../../einstein-tensor.md) in the declared convention has

$$
\delta G_{00}=2\Delta C,\qquad\delta G_{ij}=\partial_i\partial_j(A+C)-\delta_{ij}\Delta(A+C).
$$

These are also the [static scalar perturbation of Minkowski spacetime](../../../../../static-scalar-perturbation-of-minkowski-spacetime.md) equations in the original information sheet. The source has $T_{00}=M\delta^{(3)}(\mathbf x)$ and zero spatial stress. With the sign established in Question 2,

$$
\Delta C=-4\pi GM\delta^{(3)}(\mathbf x).
$$

The [distributional identity](../../../../../distributional-identity.md) $\Delta(1/\rho)=-4\pi\delta^{(3)}(\mathbf x)$ and [asymptotic flatness](../../../../../asymptotically-flat-spacetime.md) give $C=GM/\rho$. For $F=A+C$, the spatial field equation has trace $-2\Delta F=0$ and therefore $\partial_i\partial_jF=0$. Its decaying spherical solution is $F=0$, so $A=-GM/\rho$. This determines both potentials; the spatial correction cannot be inferred from the Newtonian [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) alone.

Now use the [isotropic-to-areal weak-field radius change](../../../../../isotropic-to-areal-weak-field-radius-change.md). The angular coefficient defines $r^2=(1+2GM/\rho)\rho^2$, hence $r=\rho+GM$ to first order. Thus $dr=d\rho$ to the same accuracy, and replacing $1/\rho$ by $1/r$ inside a perturbation changes only second-order terms. With the [Schwarzschild radius](../../../../../schwarzschild-radius.md) $r_S=2GM$, the [linearized Schwarzschild metric](../../../../../linearized-schwarzschild-metric.md) is

$$
\boxed{ds^2=(1-r_S/r)dt^2-(1+r_S/r)dr^2-r^2(d\theta^2+\sin^2\theta\,d\phi^2).}
$$

This is an exterior [weak-field approximation](../../../../../weak-field-approximation.md): $r_S/r\ll1$. The point source is used distributionally to fix the mass, not to claim a regular or weak field at the origin.

For a [null geodesic](../../../../../null-geodesic.md) choose its orbital plane as $\theta=\pi/2$, using rotational symmetry, and let a dot denote an [affine parameter](../../../../../affine-parameter.md) derivative. For a [Killing vector](../../../../../killing-vector-field.md) $k$ and an affinely parametrized [geodesic](../../../../../geodesic.md) tangent $U$, the [geodesic conserved quantity from a Killing vector](../../../../../geodesic-conserved-quantity-from-a-killing-vector.md) follows directly from

$$
\frac{d}{d\lambda}(k_aU^a)=U^aU^b\nabla_{(a}k_{b)}+k_a\nabla_UU^a=0.
$$

Applying this to the time-translation and axial [Killing vectors](../../../../../killing-vector-field.md), with the spatial sign absorbed into the definition of $h$, gives

$$
\boxed{E=(1-u)\dot t,\qquad h=r^2\dot\phi,\qquad u=r_S/r.}
$$

If the tangent is normalized as the photon's [four-momentum](../../../../../four-momentum.md), $E$ is its energy measured at infinity and $h$ its signed [angular momentum](../../../../../angular-momentum.md) about the selected axis. Rescaling an arbitrary [affine parameter](../../../../../affine-parameter.md) rescales both; the ratio $b=|h|/E$ is the invariant [impact parameter](../../../../../impact-parameter.md). Future-directed orbits have $E>0$. Assume $h\ne0$ to use $\phi$ as the orbit parameter; $h=0$ gives radial rays, not a finite-radius circular orbit.

The [null vector](../../../../../null-vector.md) constraint gives

$$
0=\frac{E^2}{1-u}-(1+u)\dot r^2-\frac{h^2}{r^2},\qquad \dot r^2=\frac{E^2}{1-u^2}-\frac{h^2}{r^2(1+u)}.
$$

Expand consistently to first order in the [weak-field approximation](../../../../../weak-field-approximation.md) correction: $(1-u^2)^{-1}=1+O(u^2)$ and $(1+u)^{-1}=1-u+O(u^2)$. Also $du/d\phi=-r_S\dot r/h$. Therefore the first-order orbital equation is

$$
\boxed{\left(\frac{du}{d\phi}\right)^2=\frac{r_S^2E^2}{h^2}-u^2(1-u).}
$$

The cubic term is the first correction relative to the flat inverse-radius term; the equation is not a controlled exact equation for large $u$.

A constant solution of a [first integral](../../../../../first-integral.md) is not by itself sufficient to establish a circular [geodesic](../../../../../geodesic.md). For a circular trajectory, the radial [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) also requires $A'(r)\dot t^2/2=r\dot\phi^2$, where now $A(r)=1-r_S/r$ is the metric's time coefficient. Combining this with the [null vector](../../../../../null-vector.md) constraint gives $rA'=2A$, or $u=2/3$. Equivalently, the formal potential $V(u)=u^2(1-u)$ must have a stationary point. Apart from the infinite-radius endpoint $u=0$, its only stationary point is $u_c=2/3$, with $V(u_c)=4/27$. Thus the formal circular solution requires

$$
\boxed{r_c=\frac32r_S,\qquad\left|\frac Eh\right|=\frac{2}{3\sqrt3\,r_S},\qquad b_c=\frac{3\sqrt3}{2}r_S.}
$$

The reduced radial equation is $u''=-u+\tfrac32u^2$, with prime denoting $d/d\phi$. It follows by differentiating the [first integral](../../../../../first-integral.md) on moving segments and agrees with the regular [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) at turning points. Perturbing $u=u_c+\epsilon$ gives

$$
\epsilon''=\epsilon+O(\epsilon^2),\qquad\epsilon=A_+e^\phi+A_-e^{-\phi}+O(\epsilon^2).
$$

There is an exponentially growing [linear instability](../../../../../linear-instability.md) mode; equivalently $V''(u_c)=-2<0$. **The formal circular orbit is unstable.**

<a id="3/image-the-formal-inverse-radius-photon-potential-has-its-maximum-outside-the-weak-field-regime"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-60-photon-potential.png)

**[Figure 1](#3/image-the-formal-inverse-radius-photon-potential-has-its-maximum-outside-the-weak-field-regime). The formal inverse-radius photon potential has its maximum outside the weak-field regime**.

The [weak-field photon-orbit validity](../../../../../weak-field-photon-orbit-validity.md) limitation is essential: $u_c=2/3$ is not small. There is therefore **no finite-radius circular photon orbit established within the controlled weak-field region**. The formal extrapolation happens to reproduce the radius and [impact parameter](../../../../../impact-parameter.md) of the exact Schwarzschild [photon sphere](../../../../../photon-sphere.md), but that physical result needs the exact geometry. The calculation also cannot establish a [Schwarzschild event horizon](../../../../../schwarzschild-event-horizon.md) from a first-order expansion at $u\sim1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
