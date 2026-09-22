<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In [Cartesian coordinates](../../../../cartesian-coordinate-system.md), $\nabla\Phi=(\Phi_x,\Phi_y,\Phi_z)$. For [orthogonal coordinates](../../../../orthogonal-coordinates.md), let $\mathbf r(q_1,q_2,q_3)$ be the position, $h_i=|\partial\mathbf r/\partial q_i|$ the [scale factors of orthogonal coordinates](../../../../scale-factors-of-orthogonal-coordinates.md), and $\mathbf e_i=h_i^{-1}\partial\mathbf r/\partial q_i$ the corresponding [unit vectors](../../../../unit-vector.md). Since $d\mathbf r=\sum_i h_i\mathbf e_i\,dq_i$ and $d\Phi=\nabla\Phi\cdot d\mathbf r=\sum_i\Phi_{q_i}dq_i$, comparison of independent increments gives the [gradient in orthogonal coordinates](../../../../gradient-in-orthogonal-coordinates.md):

$$
\boxed{\nabla\Phi=\sum_{i=1}^3\frac{\mathbf e_i}{h_i}\frac{\partial\Phi}{\partial q_i}.}
$$

For the [hyperbolic parametrization of oblate spheroidal coordinates](../../../../hyperbolic-parametrization-of-oblate-spheroidal-coordinates.md), the three coordinate tangent vectors are

$$
\mathbf r_R=(\sinh R\cos\theta\cos\phi,\sinh R\cos\theta\sin\phi,\cosh R\sin\theta),
$$



$$
\mathbf r_\theta=(-\cosh R\sin\theta\cos\phi,-\cosh R\sin\theta\sin\phi,\sinh R\cos\theta),\qquad\mathbf r_\phi=(-\cosh R\cos\theta\sin\phi,\cosh R\cos\theta\cos\phi,0).
$$

Their pairwise [dot products](../../../../dot-product.md) are zero. Their squared [Euclidean norms](../../../../euclidean-norm.md) are $\sinh^2R+\sin^2\theta$, $\sinh^2R+\sin^2\theta$, and $\cosh^2R\cos^2\theta$, respectively. Thus the coordinate surfaces meet orthogonally wherever this is a regular coordinate chart, and

$$
\boxed{h_R=h_\theta=\sqrt{\sinh^2R+\sin^2\theta},\qquad h_\phi=\cosh R\cos\theta.}
$$

The last expression uses the usual latitude range $|\theta|<\pi/2$; without that range a scale factor is its absolute value. Axial or ring degeneracies are excluded from a regular chart.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
