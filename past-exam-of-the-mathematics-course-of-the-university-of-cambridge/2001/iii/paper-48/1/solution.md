<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use pressure per unit constant density, $\pi$, with the [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) and [centrifugal potential](../../../../../centrifugal-potential.md) absorbed into it. [Strict geostrophic balance](../../../../../strict-geostrophic-balance.md) is the exact balance

$$
2\boldsymbol\Omega\times\mathbf u=-\nabla\pi,\qquad \nabla\cdot\mathbf u=0,
$$

with [material acceleration](../../../../../material-acceleration.md) omitted, for a homogeneous [incompressible flow](../../../../../incompressible-flow.md). Writing $f=2\Omega\ne0$, its components are $fv=\pi_x$, $fu=-\pi_y$ and $\pi_z=0$. Differentiating the first two equations with respect to $z$ gives $u_z=v_z=0$. Alternatively, the [vector calculus](../../../../../vector-calculus.md) identity

$$
\nabla\times(2\boldsymbol\Omega\times\mathbf u)=2\boldsymbol\Omega(\nabla\cdot\mathbf u)-(2\boldsymbol\Omega\cdot\nabla)\mathbf u
$$

shows, on taking the [curl](../../../../../curl.md) of the balance, that $(\boldsymbol\Omega\cdot\nabla)\mathbf u=0$. Thus $w_z=0$ too, proving the [Taylor–Proudman theorem](../../../../../taylor-proudman-theorem.md):

$$
\boxed{\pi_z=0,\qquad \mathbf u_z=0.}
$$

The physical pressure still includes its background [hydrostatic pressure](../../../../../hydrostatic-pressure.md); it is the reduced pressure $\pi$ that is independent of $z$. Between horizontal impermeable boundaries, the vertically constant $w$ is zero.

For boundaries $z=z_b(x,y)$ and $z=z_t(x,y)$, [impermeability condition](../../../../../no-penetration-boundary-condition.md) gives $w_b=\mathbf u_H\cdot\nabla_Hz_b$ and $w_t=\mathbf u_H\cdot\nabla_Hz_t$. A nearly columnar flow crossing contours of $H=z_t-z_b$ must therefore have $w_t-w_b\simeq\mathbf u_H\cdot\nabla_HH\ne0$. **Exact columnarity must give way to small corrections from [ageostrophic flow](../../../../../ageostrophic-flow.md).** The leading horizontal [geostrophic flow](../../../../../geostrophic-flow.md) can remain nearly independent of $z$, and the leading reduced pressure has $\pi_z=0$, but $w_z$ is now nonzero and exact three-dimensional [strict geostrophic balance](../../../../../strict-geostrophic-balance.md) no longer holds. For small slopes, the dominant vertical [vorticity equation](../../../../../vorticity-equation.md) is

$$
\frac{D(q+f)}{Dt}\simeq(q+f)w_z,\qquad w_z\simeq\frac1H\mathbf u_H\cdot\nabla_HH,
$$

where $q=v_x-u_y$ is [relative vorticity](../../../../../relative-vorticity.md). Equivalently, $D[(q+f)/H]/Dt\simeq0$. Crossing [geostrophic contours](../../../../../geostrophic-contour.md) stretches or squashes columns: increasing $H$ produces cyclonic relative [vorticity](../../../../../vorticity.md), decreasing $H$ produces anticyclonic relative [vorticity](../../../../../vorticity.md). The full [vorticity equation](../../../../../vorticity-equation.md) also contains tilting terms, neglected at this columnar order.

For the circular shallowing, fluid arriving from upstream has [potential vorticity](../../../../../potential-vorticity.md) $f/h$. Its height is $h(1-\epsilon)$ inside, so conservation gives

$$
\frac{f+q}{h(1-\epsilon)}=\frac fh,\qquad \boxed{q=-f\epsilon\quad(r<a),\qquad q=0\quad(r>a).}
$$

This uses the stated column-stretching description and initially open [streamlines](../../../../../streamline.md). To obtain the leading disturbance [velocity field](../../../../../velocity-field.md), use the conventional [streamfunction](../../../../../stream-function.md) definition $u=-\Psi_y$, $v=\Psi_x$, and write $\Psi=-Uy+\psi(r)$. Then $q=\nabla_H^2\psi=r^{-1}(r\psi_r)_r$. Regularity at $r=0$ gives $\psi_r=-f\epsilon r/2$ inside. Outside, $\psi_r=B/r$; matching tangential velocity at $r=a$ fixes $B=-f\epsilon a^2/2$. Choose the irrelevant additive constant so that

$$
\psi=C\begin{cases}
-r^2/2,&r<a,\\
a^2[\log(a/r)-1/2],&r>a,
\end{cases}
\qquad \boxed{C=\frac{f\epsilon}{2}=\Omega\epsilon.}
$$

Both $\psi$ and $\psi_r$ match at $a$, so there is no extra [vorticity sheet](../../../../../vortex-sheet.md) on the rim. This is the [circular topographic anticyclone](../../../../../circular-topographic-anticyclone.md). The radial expression specifies the disturbance; the **complete streamfunction is $\Psi=-Uy+\psi$**, since a radial function alone cannot represent the required uniform far-field current. Reversing the [streamfunction](../../../../../stream-function.md) sign convention reverses the displayed proportionality constant, but leaves the physical velocity unchanged.

Differentiation gives the full relative [velocity field](../../../../../velocity-field.md) in the rotating frame:

$$
(u,v)=\begin{cases}
(U+Cy,-Cx),&r<a,\\
(U+Ca^2y/r^2,-Ca^2x/r^2),&r>a,
\end{cases}
\qquad w\simeq0
$$

away from the narrow transition across the change of depth. The disturbance turns clockwise for $f\epsilon>0$ and decays as $1/r$. The horizontal field is the leading small-$\epsilon$ columnar inversion: the exact variable-depth transport across a sharp rim needs higher-order corrections, rather than an exactly two-dimensional velocity continuous across a literal vertical step.

Take $U>0$ and $\epsilon>0$. The greatest opposing zonal disturbance speed is $Ca$, attained at $(0,-a)$. If $Ca<U$, then $u>0$ everywhere and every particle advances in $x$, precluding closed [streamlines](../../../../../streamline.md). If $Ca>U$, the interior [stagnation point](../../../../../stagnation-point.md) $(0,-U/C)$ is a center, since the interior contours are circles about that point. The exterior [stagnation point](../../../../../stagnation-point.md) $(0,-Ca^2/U)$ is a saddle: linearization there has real eigenvalues of opposite sign. Closed contours around the center are bounded by a [separatrix](../../../../../separatrix.md) through the saddle. The two points meet at the rim at onset, giving the [closed-streamline threshold for a circular topographic anticyclone](../../../../../closed-streamline-threshold-for-a-circular-topographic-anticyclone.md):

$$
\boxed{Ca=U,\qquad \left(\frac\epsilon U\right)_{\rm crit}=\frac2{fa}=\frac1{\Omega a}.}
$$

At this threshold $U/(fa)=\epsilon/2\ll1$, consistent with small [Rossby number](../../../../../rossby-number.md). Equality is the onset, not a finite-area closed cell. Beyond onset, upstream data alone no longer determine the [potential vorticity](../../../../../potential-vorticity.md) of trapped fluid; the threshold follows from the continuation of the supplied open-flow model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
