<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Lift the angular coordinate continuously to a real coordinate and write $\Delta z=z_B-z_A$ and $\Delta\phi_m=\phi_B-\phi_A+2\pi m$ for a prescribed winding number $m\in\mathbb Z$. Assume $z_A<z_B$ for the calculation; reversing the endpoints changes no length. The [arc length](../../../../../arc-length.md) functional on the [circular cylinder](../../../../../circular-cylinder.md) is

$$
\mathcal L[\phi]=\int_{z_A}^{z_B}\sqrt{1+R^2\phi'(z)^2}\,dz.
$$

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) says $R^2\phi'/\sqrt{1+R^2\phi'^2}$ is constant. This expression is strictly increasing in $\phi'$, so $\phi'$ is constant. The candidate is the [helix](../../../../../helix.md)

$$
\boxed{\phi(z)=\phi_A+\frac{\Delta\phi_m}{\Delta z}(z-z_A),\qquad
\mathcal L_m=\sqrt{\Delta z^2+R^2\Delta\phi_m^2}.}
$$

It is a global minimum within the chosen winding class: the integrand is strictly [convex](../../../../../convex-function.md), and [Jensen inequality](../../../../../jensen-s-inequality.md) bounds the functional below by $(z_B-z_A)\sqrt{1+R^2(\Delta\phi_m/\Delta z)^2}$, with equality only for constant slope. Equivalently, unrolling the cylinder makes the minimizing path a straight segment.

The signed [pitch of a helix](../../../../../pitch-of-a-helix.md), measured for an increase of $2\pi$ in angle, is

$$
\boxed{P_m=\frac{2\pi\Delta z}{\Delta\phi_m}.}
$$

Its geometric magnitude is $|P_m|$. If only the physical endpoints are fixed, choose the integer $m$ minimizing $|\Delta\phi_m|$; opposite points may give two equally short helices. If the lifted endpoint angles are prescribed, use that winding class. A zero angular increment gives a straight generator, the limiting infinite-pitch case.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
