<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $B_\delta=\sqrt{\log(2m)}+\sqrt{\log(1/\delta)}$. The columns of $D^\dagger/L$ have [Euclidean norm](../../../../../../euclidean-norm.md) at most one. Under the usual [sub-Gaussian random vector](../../../../../../sub-gaussian-random-vector.md) convention, 3(d) justifies the tuning choice $\lambda=2\sqrt2 L B_\delta/n$, which is independent of $\theta^*$. Also $\|\Pi_1z\|_2=|\langle z,\mathbf1/\sqrt n\rangle|$, so the [Chernoff bound](../../../../../../chernoff-bound.md) gives $\|\Pi_1z\|_2^2\leq c_\delta=2\log(2/\delta)$ with [probability](../../../../../../probability.md) at least $1-\delta$.

On the intersection of these events, of [probability](../../../../../../probability.md) at least $1-2\delta$, set $a=\|h\|_2/\sqrt n$ and $b=\|\Pi_1z\|_2/\sqrt n$. The weighted [Young inequality](../../../../../../young-s-inequality-for-products.md) gives $2ab\leq t^2a^2+b^2/t^2$ for $0<t<1$. Applying it to 3(c) and rearranging yields the rigorous bound

$$
\boxed{\frac{\|h\|_2^2}{n}\leq\frac{4\sqrt2\,s(\theta^*)L}{n(1-t^2)}B_\delta+\frac{c_\delta}{nt^2(1-t^2)}.}
$$

If the coefficient-one concentration statement in 3(d) is taken as an extra hypothesis, instead choose $\lambda=2LB_\delta/n$; the identical argument gives precisely the printed coefficient $4$ in the first term. Thus the deterministic argument and its risk rate are sound; its concentration constants depend on correcting or strengthening 3(d).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
