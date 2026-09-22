<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For a fixed rotation axis with constant [moment of inertia](../../../../../moment-of-inertia.md), the axial [torque](../../../../../torque.md) obeys $\tau=I\ddot\theta$, with $\tau=\sum(\mathbf r\times\mathbf F)\cdot\widehat{\mathbf e}_{\rm axis}$. For a [point mass](../../../../../point-mass.md) at radius $l$, the tangential equation is $F_t=ml\ddot\theta$; multiplying by $l$ gives $lF_t=ml^2\ddot\theta$, as required. Radial [forces](../../../../../force-split.md) have zero moment about the axis.

Take increasing $\theta$ in the direction of the clapper's initial fall and let the contact [force](../../../../../force-split.md) $N$ oppose that tangential motion. Initial equilibrium of the clapper gives

$$
Nl=mgl\sin\beta,\qquad\boxed{N_{\rm initial}=mg\sin\beta.}
$$

While contact persists the bell and clapper rotate together. Their respective offsets from the upward vertical are $\theta-\beta$ and $\theta$. Summing external gravitational moments eliminates their internal contact [force](../../../../../force-split.md):

$$
\boxed{\ddot\theta=\frac{Mgh\sin(\theta-\beta)+mgl\sin\theta}{Mk^2+ml^2}.}
$$

The clapper alone satisfies $ml^2\ddot\theta=mgl\sin\theta-Nl$. Hence for $m\ll M$,

$$
\boxed{N\simeq mg\left[\sin\theta-\frac{lh}{k^2}\sin(\theta-\beta)\right].}
$$

A nonadhesive contact cannot exert tension. The first zero of this expression on the released trajectory is the loss-of-contact angle. Write $q=lh/k^2=0.9375$. Then

$$
(1-q\cos\beta)\sin\theta_0+q\sin\beta\cos\theta_0=0,
\qquad
\boxed{\theta_0=111.9^\circ.}
$$

The second-quadrant root is reached from $\theta=\beta=30^\circ$; selecting the principal negative arctangent would choose the wrong branch. Indeed the exact contact [force](../../../../../force-split.md) before taking $m/M\to0$ is $mMg[k^2\sin\theta-lh\sin(\theta-\beta)]/(Mk^2+ml^2)$, so its zero is unchanged.

## ↑ Ancestors (13)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
