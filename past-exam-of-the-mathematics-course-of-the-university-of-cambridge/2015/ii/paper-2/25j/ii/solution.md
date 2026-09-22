<h1 id="25j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Jeffreys prior](../../../../../../jeffreys-prior.md) is proportional to $[\theta(1-\theta)]^{-1/2}$, hence is $\operatorname{Beta}(1/2,1/2)$. Its posterior is $\operatorname{Beta}(X+1/2,n-X+1/2)$, giving

$$
\boxed{\mathbb E[\theta\mid X]=\frac{X+1/2}{n+1},\qquad m_{\theta\mid X}=\begin{cases}0&X=0,\\(X-1/2)/(n-1)&0<X<n,\\1&X=n.\end{cases}}
$$

The interior case is used only when $n\geq2$. Generally neither rule equals $X/n$: the mean agrees only at $X=n/2$; the mode agrees at the endpoints and, in the interior, at $X=n/2$. For the small experiments $n=1,2$, all possible observations happen to be among these cases, so the whole mode rule then coincides with the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [25J](../../25j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
