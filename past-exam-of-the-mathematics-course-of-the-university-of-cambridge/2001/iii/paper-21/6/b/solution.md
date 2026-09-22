<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When paths move only by jumps of size $\pm1$, there is neither a Gaussian component nor a continuous drift. The [Lévy measure](../../../../../../levy-measure.md) is supported on $\{-1,1\}$ and has finite mass because these points are bounded away from zero. The process is therefore a [Compound Poisson process](../../../../../../compound-poisson-process.md), expressible as a [difference of independent Poisson processes](../../../../../../difference-of-independent-poisson-processes.md)

$$
X_t=N_t^+-N_t^-,
$$

where the rates are $\lambda_+,\lambda_-$ respectively. The martingale assumptions imply

$$
0=\mathbb E X_t=(\lambda_+-\lambda_-)t,\qquad
\operatorname{Var}(X_t)=(\lambda_++\lambda_-)t=t.
$$

Hence $\boxed{\lambda_+=\lambda_-=1/2}$. The embedded jump chain is a [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md), and the total jump rate is one. In particular,

$$
\boxed{X_1\overset d=N_+-N_-,\qquad N_+,N_-\text{ independent Poisson}(1/2).}
$$

This is the symmetric [Skellam distribution](../../../../../../skellam-distribution.md), with the explicit mass function

$$
\boxed{\mathbb P(X_1=k)=e^{-1}\sum_{j=0}^{\infty}\frac{2^{-(2j+|k|)}}{j!(j+|k|)!},\qquad k\in\mathbb Z.}
$$

For $k\geq0$, sum the joint probabilities of $N_+=j+k,N_-=j$; for $k<0$, interchange the two variables. The [characteristic function](../../../../../../characteristic-function.md) is $\mathbb E e^{iuX_1}=\exp(\cos u-1)$, consistent with the rate-one [symmetric Poisson difference process](../../../../../../symmetric-poisson-difference-process.md). The condition that paths move only by jumps is essential to exclude a separate continuous component.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
