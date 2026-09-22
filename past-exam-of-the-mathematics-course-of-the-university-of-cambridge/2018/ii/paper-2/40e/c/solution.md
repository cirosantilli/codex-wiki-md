<h1 id="40e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [stationary iterative method for a linear system](../../../../../../stationary-iterative-method-for-a-linear-system.md) converges from every initial vector exactly when the [spectral radius](../../../../../../spectral-radius.md) of its [iteration matrix](../../../../../../iteration-matrix.md) is less than one. Here $\cos(kx)$ ranges between $\cos x$ and $-\cos x$, so all modes decay for a fixed $n$ exactly when

$$
-1<1-\omega-\omega\cos x
\leq\lambda_k(\omega)
\leq1-\omega+\omega\cos x<1.
$$

Requiring this for every grid size gives

$$
\boxed{0<\omega\leq1.}
$$

Indeed, $\omega\leq0$ leaves or amplifies the lowest mode, while any $\omega>1$ makes the highest-mode eigenvalue tend to $1-2\omega<-1$ as $n\to\infty$.

The slowest mode is $k=1$, for which the [Taylor expansion](../../../../../../taylor-expansion.md) is

$$
\lambda_1(\omega)
=1-\omega+\omega\cos\frac{\pi}{n+1}
=1-\frac{\omega\pi^2}{2(n+1)^2}
+O(n^{-4}).
$$

If the initial error has a nonzero $\mathbf v_1$ component, that component is multiplied by $\lambda_1(\omega)^\nu$. Hence for a constant $c>0$ independent of $n$,

$$
\boxed{\|\mathbf e^{(\nu)}\|
\ \text{cannot in general decay faster than}\
\left(1-\frac{c}{n^2}\right)^\nu.}
$$

This is the low-frequency obstruction to grid-independent convergence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
