<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $h_x=1/(N+1)$ and $J=2N+1$. The [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) has the [eigenvectors](../../../../../../eigenvector.md)

$$
 v_j(m)=\sin\frac{j\pi(m+N+1)}{2N+2},\qquad j=1,\ldots,2N+1,
$$

and its negative has the [eigenvalues](../../../../../../eigenvalue.md)

$$
 \lambda_j^h=\frac4{h_x^2}\sin^2\frac{j\pi}{4(N+1)}.
$$

The [discrete sine transform](../../../../../../discrete-sine-transform.md) therefore reduces the [method of lines](../../../../../../method-of-lines.md) equations to $q_j''=(\alpha-\lambda_j^h)q_j$. Each coefficient is an oscillator, a linear function, or a hyperbolic function according to the sign of $\lambda_j^h-\alpha$. A finite collection of oscillators is bounded in every fixed-grid [norm](../../../../../../norm.md). A zero-frequency mode can grow linearly, and a negative-frequency-square mode can grow exponentially. Consequently,

$$
\boxed{\alpha<4(N+1)^2\sin^2\frac{\pi}{4(N+1)}}
$$

is necessary and sufficient for [all-time boundedness of a semidiscrete reaction wave equation](../../../../../../all-time-boundedness-of-a-semidiscrete-reaction-wave-equation.md) on this grid. Equality allows bounded displacement only when the initial velocity has zero projection onto the first [eigenvector](../../../../../../eigenvector.md); above it, the growing components must be absent in every unstable mode. A strictly positive [spectral gap](../../../../../../spectral-gap.md) also gives a time-independent displacement bound uniform over grids whose gaps are bounded below.

The discrete threshold is strictly smaller than $\pi^2/4$, because $\sin s<s$ for $s>0$, and tends to $\pi^2/4$ as $N\to\infty$. A coarse grid can therefore introduce long-time growth into a continuum problem with $\alpha<\pi^2/4$. This is distinct from [displacement stability of a symmetric semidiscrete wave equation](../../../../../../displacement-stability-of-a-symmetric-semidiscrete-wave-equation.md) on fixed finite time intervals. As in part (a), if existence of the printed limit is required for every initial datum, **no $\alpha$ qualifies**: any one mode admits oscillatory, secular, or growing initial data, depending on its coefficient.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
