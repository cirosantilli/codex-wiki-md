<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $S=n_{11}+n_{22}$, $R=n_{12}+n_{21}$ and $N=S+R$. With equal positive rates, the one-year [probability](../../../../../../../probability.md) of a change is $q(\lambda)=(1-e^{-2\lambda})/2\in(0,1/2)$, so the conditional [likelihood function](../../../../../../../likelihood-function.md) is proportional to

$$
(1-q)^Sq^R.
$$

For $N>0$, its unrestricted binomial maximizer is $q=R/N$. A finite interior positive-rate maximum exists exactly when $0<R/N<1/2$, or

$$
\boxed{0<R<S,\qquad \widehat\lambda=\frac12\log\frac{S+R}{S-R}.}
$$

Indeed the binomial [log-likelihood](../../../../../../../log-likelihood.md) is strictly concave at this interior maximum and $q(\lambda)$ is strictly increasing. If $R\geq S$ and $R>0$, the likelihood increases towards its supremum as $q\uparrow1/2$, requiring $\lambda\to\infty$; no finite maximum exists. Equality $R=S>0$ also has only this limiting maximum.

If $R=0<S$, allowing the boundary $\lambda=0$ gives a finite maximum there; insisting on $\lambda>0$ gives only a supremum as $\lambda\downarrow0$. Thus if “valid” includes zero rates, the condition is $R<S$ with $N>0$; if rates must be strictly positive, it is $0<R<S$. If $N=0$, every rate has the same empty-data likelihood and the [statistical parameter](../../../../../../../statistical-parameter.md) is not identifiable. These boundary qualifications prevent a negative or infinite plug-in rate from being called a valid interior estimate.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
