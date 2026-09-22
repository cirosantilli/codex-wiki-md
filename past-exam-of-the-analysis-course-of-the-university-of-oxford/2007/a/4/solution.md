<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [spectrum of a bounded operator](../../../../spectrum-of-a-bounded-operator.md) consists of $\lambda$ for which $T-\lambda I$ has no bounded two-sided inverse. The [point spectrum](../../../../point-spectrum.md) consists of [eigenvalues](../../../../eigenvalue.md), so $\ker(T-\lambda I)\ne0$. The [approximate point spectrum](../../../../approximate-point-spectrum.md) consists of $\lambda$ admitting [unit vectors](../../../../unit-vector.md) $x_n$ with $\|(T-\lambda I)x_n\|\to0$; equivalently $T-\lambda I$ is not bounded below.

If $T-\lambda I$ is invertible, its inverse bounds it below and its [Banach-space adjoint](../../../../transpose-of-a-bounded-linear-operator.md) is invertible. Thus neither alternative on the right of the claimed union occurs. Conversely suppose $\lambda$ belongs to neither term and write $S=T-\lambda I$. There is $c>0$ with $\|Sx\|\geq c\|x\|$, so $S$ is injective and has closed range: convergence of $Sx_n$ makes $x_n$ Cauchy, and [completeness](../../../../completeness.md) supplies a preimage of its limit. Also $\ker S'=0$. The allowed annihilator identity makes the range dense, hence equal to $X$. Its inverse has [norm](../../../../norm.md) at most $1/c$. This proves the [spectrum decomposition through the Banach-space adjoint](../../../../spectrum-decomposition-through-the-banach-space-adjoint.md):

$$
\boxed{\sigma(T)=\operatorname{ap}\sigma(T)\cup\operatorname p\sigma(T').}
$$

For the right shift on $\ell^1$, $\|T\|=1$, so the allowed [norm](../../../../norm.md) bound puts its spectrum in the closed unit disc. Under the linear pairing with $\ell^\infty$, its [Banach-space adjoint](../../../../transpose-of-a-bounded-linear-operator.md) is the left shift $T'(b_1,b_2,\ldots)=(b_2,b_3,\ldots)$. For each $|\lambda|\leq1$ the bounded nonzero sequence $(1,\lambda,\lambda^2,\ldots)$ is an [eigenvector](../../../../eigenvector.md) of $T'$ with [eigenvalue](../../../../eigenvalue.md) $\lambda$. The union identity gives the reverse inclusion. Hence **$\sigma(T)=\{\lambda:|\lambda|\leq1\}$**. This [Banach-space adjoint](../../../../transpose-of-a-bounded-linear-operator.md) uses the complex-linear dual, so its [eigenvalue](../../../../eigenvalue.md) is $\lambda$ itself.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
