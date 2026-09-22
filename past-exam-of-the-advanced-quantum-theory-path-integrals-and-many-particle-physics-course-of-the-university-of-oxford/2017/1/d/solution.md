<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Insert the decorating-spin [observable](../../../../observable.md) into the one bond that contains it. The [decorated-spin occupation insertion](../../../../decorated-spin-occupation-insertion.md) uses the [matrix](../../../../matrix.md):

$$
Q_{st}=\sum_{t_0=-1}^{1}t_0^2e^{Kt_0(s+t)}=2\cosh[K(s+t)]
=\begin{pmatrix}2\cosh2K&2\\2&2\cosh2K\end{pmatrix}_{st}.
$$

The [partition function](../../../../canonical-partition-function.md) still contains $L$ decorating-spin sums; one of them has been replaced by this weighted sum. Hence

$$
\langle\tau_1^2\rangle_L=\frac{\operatorname{tr}(QV^{L-1})}{Z_L}
=\frac{q_+\lambda_+^{L-1}+q_-\lambda_-^{L-1}}{\lambda_+^L+\lambda_-^L},
\qquad q_+=2\cosh2K+2,\quad q_-=2\cosh2K-2.
$$

Taking the dominant [eigenvector](../../../../eigenvector.md) gives

$$
\boxed{\lim_{L\to\infty}\langle\tau_1^2\rangle_L=\frac{q_+}{\lambda_+}
=\frac{\cosh2K+1}{\cosh2K+2}=\frac{2\cosh^2K}{1+2\cosh^2K}.}
$$

This is the [probability](../../../../probability.md) that the decorating site is in either nonzero state. It tends to $2/3$ at high [temperature](../../../../temperature-split.md), when its three states are equally likely, and to one at low [temperature](../../../../temperature-split.md), when the nonzero aligned states gain [bond energy](../../../../energy-split.md). Unlike the [magnetization](../../../../magnetization.md), this even [observable](../../../../observable.md) is not forced to vanish by [spin](../../../../spin.md) reversal.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
