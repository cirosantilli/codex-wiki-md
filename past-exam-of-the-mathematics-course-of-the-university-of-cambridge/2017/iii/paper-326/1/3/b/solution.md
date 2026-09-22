<h1 id="1/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Picard criterion](../../../../../../../picard-criterion.md) with the input/output convention above states

$$
\boxed{f\in\mathcal R(K)\iff f\in\overline{\mathcal R(K)}\ \text{and}\ \sum_j\frac{|\langle f,v_j\rangle|^2}{\sigma_j^2}<\infty.}
$$

Necessity follows from $\langle f,v_j\rangle=\sigma_j\langle u,u_j\rangle$ and [Bessel inequality](../../../../../../../bessel-s-inequality.md). Conversely the summability constructs $u=\sum_j\sigma_j^{-1}\langle f,v_j\rangle u_j\in U$; the closure condition ensures that its image is all of $f$. The closure condition must not be omitted: a component orthogonal to the range cannot be reconstructed.

For the diagonal example, $f_j=j^{-p}$ is itself in $\ell^2$ only for $p>1/2$. Its preimage would be $u_j=j^{1-p}$, so the range criterion is the convergence of $\sum_jj^{2-2p}$. The [P-series](../../../../../../../p-series.md) gives

$$
\boxed{f\in\mathcal R(K)\iff p>3/2.}
$$

At $p=3/2$ the reconstruction [norm](../../../../../../../norm.md) diverges harmonically. For $1/2<p\leq3/2$ the data are legitimate but have no preimage; for $0<p\leq1/2$ they are not even in the specified data space.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
