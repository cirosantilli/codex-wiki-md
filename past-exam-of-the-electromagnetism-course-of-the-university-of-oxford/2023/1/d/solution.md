<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Translate the concentric spheres so that their centre is $(0,0,-a)$, take $b=a+d$, and keep the [point charge](../../../../point-charge.md) fixed at $(0,0,h)$. Its distance from the centre is $r_0=a+h$. As $a\to\infty$, the upper portions of the inner and outer spheres approach the planes $z=0$ and $z=d$. The preceding total induced [electric charge](../../../../electric-charge-split.md) becomes

$$
Q_a=-q\frac{a(d-h)}{(a+h)d}\longrightarrow-\frac{q(d-h)}d.
$$

The outer sphere has total induced [electric charge](../../../../electric-charge-split.md) $Q_b=-q-Q_a$: a [Gaussian surface](../../../../gaussian-surface.md) within its conducting material has zero [electric flux](../../../../electric-flux.md), and the grounded exterior is field-free by [uniqueness of Poisson equation](../../../../uniqueness-of-poisson-equation.md). Therefore $Q_b\to-qh/d$.

One can justify the total-charge limit without assuming that local convergence of [electric fields](../../../../electric-field-split.md) preserves their [surface integrals](../../../../surface-integral.md). Use [induced charge as harmonic measure](../../../../induced-charge-as-harmonic-measure.md): if a [harmonic function](../../../../harmonic-function.md) $w$ is one on the selected grounded boundary and zero on the other, [Green's second identity](../../../../green-second-identity.md) with the [electric potential](../../../../electric-potential.md) gives

$$
Q_{\rm selected}=-q\,w(\mathbf r_0).
$$

Indeed, $\nabla^2\phi=-q\delta^{(3)}(\mathbf r-\mathbf r_0)/\epsilon_0$, $\phi=0$ on the boundaries, and their [unit normal](../../../../unit-normal.md) outward from the gap satisfies $\sigma=\epsilon_0\partial_n\phi$. For the spheres the weighting [harmonic function](../../../../harmonic-function.md) is $w_a(r)=a(b-r)/(r(b-a))$, exactly the factor already obtained. For the slab the two weighting [harmonic functions](../../../../harmonic-function.md) are $w_0=1-z/d$ and $w_d=z/d$. Applying the same identity to the decaying grounded-slab [electric potential](../../../../electric-potential.md), whose boundary term at lateral infinity vanishes, establishes directly

$$
\boxed{Q_0=-\frac{q(d-h)}d,\qquad Q_d=-\frac{qh}d.}
$$

Their sum is $-q$, and their relative sizes measure how close the [point charge](../../../../point-charge.md) lies to each grounded plane.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the electromagnetism course of the University of Oxford](../../../split.md)
5. [Electromagnetism course of the University of Oxford](../../../../electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
