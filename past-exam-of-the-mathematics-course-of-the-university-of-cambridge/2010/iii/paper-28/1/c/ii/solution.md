<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $r=q/p>1$ and $H_k$ be the first [hitting time](../../../../../../../first-passage-time.md) of level $k$. Nearest-neighbour steps imply $S_{H_k}=k$ whenever $H_k<\infty$: the walk cannot overshoot its first upward crossing. On this event the stopped [martingale](../../../../../../../martingale-split.md) eventually has the constant value $r^k$. On $\{H_k=\infty\}$, it is $Z_n$ and tends to zero by part (i). Therefore

$$
\boxed{Z_{n\wedge H_k}\longrightarrow r^k\mathbf1_{\{H_k<\infty\}}
=e^{\lambda_k}\mathbf1_{\{H_k<\infty\}},\qquad\lambda_k=k\log(q/p).}
$$

For every $n$, $0\leq Z_{n\wedge H_k}\leq r^k$. Before the hit the walk is below $k$, and at the hit it equals $k$. The [optional stopping theorem](../../../../../../../optional-sampling-theorem-for-a-supermartingale.md) for the bounded [stopping time](../../../../../../../stopping-time.md) $n\wedge H_k$ gives $\mathbb EZ_{n\wedge H_k}=\mathbb EZ_0=1$. The [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md) now yields $1=r^k\mathbb P(H_k<\infty)$. Consequently

$$
\boxed{\mathbb P(H_k<\infty)=(p/q)^k.}
$$

The uniform bound on the stopped variables justifies the limit; applying optional stopping directly at the possibly infinite $H_k$ without this argument would not be valid.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
