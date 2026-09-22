# Nested-disk subtraction for paraboloid volumes

↑ **Parent:** [Elliptic paraboloid](elliptic-paraboloid.md)

Suppose a solid is above the [elliptic paraboloid](elliptic-paraboloid.md) $z=x^2+y^2$ and below a [plane](plane.md) whose vertical separation from it is $A-|\mathbf x-\mathbf p|^2$, where $A>0$. A second lower [plane](plane.md) exceeds the [elliptic paraboloid](elliptic-paraboloid.md) by $B-|\mathbf x-\mathbf q|^2$, with $B>0$. If $|\mathbf p-\mathbf q|+\sqrt B\leq\sqrt A$, the [disk](disk-mathematics.md) where the lower [plane](plane.md) matters lies within the upper [projection](projection-linear-algebra.md). Raising the bottom to this lower [plane](plane.md) therefore removes exactly its excess [volume](volume.md), without changing the outer [projection](projection-linear-algebra.md).

Translate [polar coordinates](polar-coordinates.md) separately to the two centres. The [double integral](double-integral.md) over a [disk](disk-mathematics.md) of squared radius $A$ is

$$
\int_0^{2\pi}\int_0^{\sqrt A}(A-r^2)r\,dr\,d\theta=\frac{\pi A^2}{2}.
$$

Subtracting the analogous [integral](integral-split.md) with $B$ proves the displayed [volume](volume.md) formula. The containment condition is essential: if the two [disks](disk-mathematics.md) overlap only partly, subtract only over their intersection.

## ↑ Ancestors (6)

1. [Elliptic paraboloid](elliptic-paraboloid.md)
2. [Euclidean geometry](euclidean-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-v-resit/question-3/c/solution.md)
