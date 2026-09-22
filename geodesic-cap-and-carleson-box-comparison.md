# Geodesic-cap and Carleson-box comparison

↑ **Parent:** [Hyperbolic geodesic cap](hyperbolic-geodesic-cap.md)

For a short arc $I$ of normalized length $\ell$, every point of its [hyperbolic geodesic cap](hyperbolic-geodesic-cap.md) lies within Euclidean distance $C\ell$ of its center boundary point. Conversely, for any fixed $b>0$, the region with angular projection in $I$ and depth $1-|z|\le b\ell$ lies in $Q(\kappa I)$ for a fixed enlargement $\kappa$ depending only on $b$, when $I$ is sufficiently short. To verify this, rotate the midpoint to one and write the endpoints as $e^{\pm i\alpha}$. The cap inequality is $2\operatorname{Re}z>(1+|z|^2)\cos\alpha$. Its radial depth at the midpoint is $1-\sec\alpha+\tan\alpha$, comparable to $\alpha$ for small $\alpha$; its angular projection lies in $I$. Enlarging $\alpha$ by a sufficiently large fixed factor makes the inequality hold throughout the indicated rectangle. Large arcs use a finite cover of the disc. Thus [Carleson boxes](carleson-box.md) and [hyperbolic geodesic caps](hyperbolic-geodesic-cap.md) define equivalent [Carleson measure](carleson-measure.md) conditions.

The rectangle containment can also be checked directly. Write $z=re^{i\theta}$ with $|\theta|\le\pi\ell$ and $1-r\le b\ell$. Its membership in the enlarged cap is equivalent to

$$
\cos\theta-\cos(\kappa\pi\ell)>\frac{(1-r)^2}{2r}\cos(\kappa\pi\ell).
$$

For small enough $\ell$, $r\ge1/2$. The right side is at most $b^2\ell^2$, while the left side is at least $(\kappa^2-1)\pi^2\ell^2/8$, using the sine product formula and $\sin x\ge x/2$ for small positive $x$. Thus $\kappa=4+4b/\pi$ suffices.

## ↑ Ancestors (8)

1. [Hyperbolic geodesic cap](hyperbolic-geodesic-cap.md)
2. [Hyperbolic distance in the Poincare disc](hyperbolic-distance-in-the-poincare-disc.md)
3. [Poincaré disk model](poincare-disk-model.md)
4. [Hyperbolic geometry](hyperbolic-geometry.md)
5. [Geometry and topology](geometry-and-topology-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Carleson embedding theorem on the disk](carleson-embedding-theorem-on-the-disk.md)
- [Carleson measure](carleson-measure.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-9/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-9/5/b/solution.md)
