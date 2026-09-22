<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the corrected same-node method identified above, with $\delta=1/M$, interior indices $1,\ldots,M-1$ and zero endpoint values. Its spatial [matrix](../../../../../../matrix.md) $L_\delta$ is real symmetric. Summation by parts gives, for a vector extended by zero at the endpoints,

$$
-v^TL_\delta v=\delta^{-2}\sum_{j=0}^{M-1}a_{j+1/2}(v_{j+1}-v_j)^2.
$$

Hence $-L_\delta$ is positive definite, and $\sum_j(v_{j+1}-v_j)^2\leq4\sum_jv_j^2$ bounds its [eigenvalues](../../../../../../eigenvalue.md) by $4a_+/\delta^2$. The [Forward Euler method](../../../../../../euler-method.md) has amplification [matrix](../../../../../../matrix.md) $I+kL_\delta$. Its [eigenvalues](../../../../../../eigenvalue.md) lie in $[1-4\mu a_+,1]$, so their moduli are at most one when

$$
\boxed{0<\mu\leq\frac1{2a_+}.}
$$

Symmetry makes this a contraction in the mesh-weighted [discrete L2 norm](../../../../../../discrete-l2-norm.md), uniformly over all grids and all coefficient samples satisfying the bounds. There is also a [maximum norm](../../../../../../supremum-norm.md) proof: the update weights are $\mu a_{m-1/2}$, $1-\mu(a_{m-1/2}+a_{m+1/2})$, and $\mu a_{m+1/2}$. They are nonnegative and sum to one, giving a contraction after the boundary values are included.

This mesh-independent bound is sharp. For $a\equiv a_+$, the spatial eigenvectors are $\sin(j\pi m/M)$ and their amplification factors are

$$
1-4\mu a_+\sin^2\frac{j\pi}{2M},\qquad j=1,\ldots,M-1.
$$

If $\mu>1/(2a_+)$, sufficiently fine grids have a highest-frequency factor below $-1$, giving exponential growth in the step number.

On one fixed grid, rather than uniformly under refinement, the sharp universal [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) bound in the [discrete L2 norm](../../../../../../discrete-l2-norm.md) is slightly larger:

$$
\mu\leq\frac1{2a_+\cos^2(\pi/(2M))}.
$$

Indeed the quadratic form above is bounded by $a_+$ times the constant-coefficient difference form, whose largest [eigenvalue](../../../../../../eigenvalue.md) is $4\cos^2(\pi/(2M))/\delta^2$; equality is realized by the constant coefficient. Its limit as $M\to\infty$ is the boxed bound. No such fixed-grid [matrix](../../../../../../matrix.md) conclusion repairs the ill-defined shifted-boundary update in the literal printed formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
