<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

Two real symmetric [bilinear forms](../../../../../bilinear-form.md) are congruent if an invertible [linear map](../../../../../linear-map.md) takes one to the other; in matrices, $B=S^{\mathsf T}AS$ for some invertible $S$. The [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives an orthogonal eigenbasis. Rescaling each basis vector with nonzero eigenvalue then reduces any such form to

$$
\operatorname{diag}(I_p,-I_q,0_r),\qquad p+q+r=n.
$$

[Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) asserts that $(p,q,r)$ is independent of the congruence reduction. To prove it, $p$ is the greatest dimension of a subspace on which the form is positive definite: the positive coordinate subspace attains it, whereas any subspace of dimension greater than $p$ meets the nonpositive coordinate subspace of dimension $n-p$ and therefore cannot be positive definite. Applying the same argument to the negative of the form determines $q$. Then $r=n-p-q$ is determined too.

The [rank of a quadratic form](../../../../../rank-of-a-quadratic-form.md) is $p+q$, and its [signature of a quadratic form](../../../../../signature-of-a-quadratic-form.md) is $p-q$ under the signed-difference convention. They determine $p,q,r$ and hence the congruence class. Counting all pairs $p,q\geq0$ with $p+q\leq n$ gives

$$
\boxed{\text{number of classes}=\sum_{p=0}^n(n-p+1)=\frac{(n+1)(n+2)}2.}
$$

For $n\geq1$, **exactly two classes have every level set bounded**: the positive-definite and negative-definite classes. Their nonempty nonzero levels are ellipsoids, and their zero level is the origin. A degenerate form has an entire null line in its zero level. An indefinite nondegenerate form also has a nonzero isotropic vector, for example the sum of one positive and one negative normalized basis vector, whose scalar multiples make the zero level unbounded.

For the displayed three-dimensional form,

$$
A=\begin{pmatrix}3&2&1\\2&6&4\\1&4&5\end{pmatrix}.
$$

Its leading principal minors are $3,14,32$, all positive. [Sylvester's criterion](../../../../../sylvester-s-criterion.md) makes it positive definite, so **the surface is a bounded ellipsoid**. Directly, its quadratic expression is

$$
3\left(x+\frac23y+\frac13z\right)^2
+\frac{14}{3}\left(y+\frac57z\right)^2+\frac{16}{7}z^2,
$$

which also proves positivity and boundedness of the unit level.

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
