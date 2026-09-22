<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $P=\omega\omega^T$. Since $P^T=P$ and $P^2=P$, the [orthogonal reflection](../../../../reflection-in-a-hyperplane.md) $R_\omega=I-2P$ satisfies $R_\omega^TR_\omega=I$ and $R_\omega^{-1}=R_\omega$. Thus, for every [Borel set](../../../../borel-set.md) $E$, invariance under the [orthogonal group](../../../../orthogonal-group.md) gives

$$
(R_\omega{}_\#\mu)(E)=\mu(R_\omega^{-1}E)=\mu(E),\qquad\boxed{R_\omega{}_\#\mu=\mu.}
$$

**The spherical average must use normalized surface measure without an additional area factor.** Let $d\sigma$ be the normalized [surface measure on a sphere](../../../../surface-measure-on-a-sphere.md), and set

$$
A\eta(r)=\int_{\mathbb S^{d-1}}\eta(r\theta)\,d\sigma(\theta).
$$

The correct [radial disintegration of an orthogonally invariant measure](../../../../radial-disintegration-of-an-orthogonally-invariant-measure.md) is

$$
\boxed{\int\eta(x)\,d\mu(x)=\int_{[0,\infty)}A\eta(r)\,d(\Phi_\#\mu)(r).}
$$

Indeed, take normalized [Haar measure](../../../../haar-measure.md) $H$ on the compact [orthogonal group](../../../../orthogonal-group.md) $O(d)$. Invariance and [Fubini's theorem](../../../../fubini-s-theorem.md) give

$$
\int\eta\,d\mu=\int\!\int_{O(d)}\eta(Qx)\,dH(Q)\,d\mu(x).
$$

Right invariance of [Haar measure](../../../../haar-measure.md) and transitivity of the [orthogonal group](../../../../orthogonal-group.md) on each [sphere](../../../../sphere.md) show that the inner average depends only on $r=|x|$. Averaging it once more over $x=r\theta$, using invariance of [surface measure on a sphere](../../../../surface-measure-on-a-sphere.md) and [Fubini's theorem](../../../../fubini-s-theorem.md), identifies its value as $A\eta(r)$. At $x=0$ the same identity reads $\eta(0)=\eta(0)$. The definition of [pushforward measure](../../../../pushforward-measure.md) now proves the boxed formula. This argument also works for invariant [probability measures](../../../../probability-measure.md) with an [atom of a measure](../../../../atom-measure-theory.md) at the origin.

For the printed normalization, choose a [smooth cutoff function](../../../../smooth-cutoff-function.md) $\eta$ equal to one on a ball containing the [support of a measure](../../../../support-of-a-measure.md) $\mu$. Its left integral is one, whereas the printed right integral is $\sigma_d$. Thus the extra $\sigma_d$ cannot be retained. Equivalently, with unnormalized area measure $dS$, the average is $\sigma_d^{-1}\int\eta(r\theta)\,dS(\theta)$.

**The reflection-averaging hint also fails in general dimension.** For $x=e_1$,

$$
\int_{\mathbb S^{d-1}}R_\omega e_1\,d\sigma(\omega)=\left(1-\frac2d\right)e_1,
\qquad\int_{\mathbb S^{d-1}}\omega\,d\sigma(\omega)=0.
$$

The first equality uses $\int\omega_i\omega_j\,d\sigma=\delta_{ij}/d$, which follows from coordinate reflections, coordinate permutations, and $\sum_i\omega_i^2=1$. Taking a [test function](../../../../test-function.md) equal to the first coordinate near the unit [sphere](../../../../sphere.md) disproves the hint when $d\ne2$. Averaging over the full [orthogonal group](../../../../orthogonal-group.md), as above, proves the required corrected result without that hint.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
