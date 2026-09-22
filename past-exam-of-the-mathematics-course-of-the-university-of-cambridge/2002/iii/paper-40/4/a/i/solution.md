<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $v=\sigma^2>0$, $\bar x=n^{-1}\sum_i x_i$ and $S=\sum_i(x_i-\bar x)^2$. The [likelihood function](../../../../../../../likelihood-function.md) and [log-likelihood](../../../../../../../log-likelihood.md) are

$$
L(\mu,v)=(2\pi v)^{-n/2}\exp\left[-\frac{S+n(\mu-\bar x)^2}{2v}\right],\qquad
\ell(\mu,v)=-\frac n2\log(2\pi v)-\frac{S+n(\mu-\bar x)^2}{2v}.
$$

For every fixed $v$, the unique maximum in $\mu$ is $\bar x$. At that value, $\partial\ell/\partial v=-n/(2v)+S/(2v^2)$ changes sign from positive to negative at $v=S/n$. Thus, for $S>0$,

$$
\boxed{\widehat\mu=\bar x,\qquad\widehat{\sigma^2}=S/n.}
$$

This is the global [maximum-likelihood estimate](../../../../../../../maximum-likelihood-estimator.md), since the first maximization was global for each $v$ and the second has a unique peak. If $S=0$, the [likelihood function](../../../../../../../likelihood-function.md) is unbounded at $\mu=\bar x$, $v\downarrow0$; there is no maximizer in the parameter space $v>0$. The freezing argument below uses the nondegenerate case $S>0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
