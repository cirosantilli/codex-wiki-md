<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [closest point theorem in a Hilbert space](../../../../../../hilbert-projection-theorem.md) says that, for every nonempty closed [convex set](../../../../../../convex-set.md) $C\subset H$ and $x\in H$, there is exactly one $p\in C$ minimizing $\|x-p\|$.

Put $d=\inf_{y\in C}\|x-y\|$ and choose $y_n\in C$ with $\|x-y_n\|\to d$. The midpoint belongs to $C$ because it is a [convex set](../../../../../../convex-set.md). The [parallelogram law](../../../../../../parallelogram-law.md) gives

$$
\|y_n-y_m\|^2
=2\|x-y_n\|^2+2\|x-y_m\|^2-4\left\|x-\frac{y_n+y_m}{2}\right\|^2
\leq2\|x-y_n\|^2+2\|x-y_m\|^2-4d^2\longrightarrow0.
$$

Thus $(y_n)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). Completeness of the [Hilbert space](../../../../../../hilbert-space-split.md) and closedness of $C$ give a limit $p\in C$, with $\|x-p\|=d$. Applying the same identity to two minimizers gives their squared distance at most zero, proving uniqueness.

The resulting projection is characterized by

$$
\boxed{\operatorname{Re}\langle x-p,z-p\rangle\leq0\quad(z\in C).}
$$

Indeed, differentiate $\|x-p-t(z-p)\|^2$ at $t=0^+$; the minimum there gives the inequality. Conversely, expanding $\|x-z\|^2$ proves minimality from this inequality. For a closed linear subspace, both signs of each direction are allowed, so $x-p$ is [orthogonal](../../../../../../orthogonal-vectors.md) to that subspace: this recovers the [orthogonal projection](../../../../../../orthogonal-projection.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
