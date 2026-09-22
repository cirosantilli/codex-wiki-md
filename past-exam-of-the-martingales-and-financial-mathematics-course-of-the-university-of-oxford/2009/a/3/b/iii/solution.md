<h1 id="a/3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applies to $M$ at the bounded [stopping time](../../../../../../stopping-time.md) $n\wedge T_k$. As $M_0=0$, it yields the valid [stopped second-moment identity for a simple symmetric random walk](../../../../../../stopped-second-moment-identity-for-a-simple-symmetric-random-walk.md)

$$
\boxed{\mathbb E S_{n\wedge T_k}^2=\mathbb E(n\wedge T_k).}
$$

**The printed bound on $\mathbb E T_k$ is false.** Before hitting the positive level $k$, the walk can travel arbitrarily far downwards, so $|S_{n\wedge T_k}|\leq k$ is unavailable.

Here is a valid proof of finiteness of $T_k$. For a positive integer $L$, stop instead at $\tau=\inf\{n:S_n\in\{-L,k\}\}$. The same identity and the bound $|S_{n\wedge\tau}|\leq\max(L,k)$ give

$$
\mathbb E(n\wedge\tau)\leq\max(L,k)^2.
$$

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) makes $\mathbb E\tau<\infty$, so $\tau<\infty$ almost surely. Applying [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $S$ at $n\wedge\tau$ and then using [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives $\mathbb E S_\tau=0$. Since $S_\tau\in\{-L,k\}$, this means

$$
\mathbb P(S_\tau=k)=\frac L{L+k}.
$$

Consequently $\mathbb P(T_k<\infty)\geq L/(L+k)$ for every $L$, and letting $L\to\infty$ proves $T_k<\infty$ almost surely.

In fact this is the [infinite mean first passage of a simple symmetric random walk](../../../../../../infinite-mean-first-passage-of-a-simple-symmetric-random-walk.md). If $\mathbb E T_k<\infty$, the first displayed identity would bound the second moments of $S_{n\wedge T_k}$ uniformly. Their [uniform integrability](../../../../../../uniform-integrability.md) and their almost sure convergence to $k$ would imply $\mathbb E S_{n\wedge T_k}\to k$. But the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to $S$ at every bounded $n\wedge T_k$ makes each expectation zero, a contradiction. Hence the correct conclusion is

$$
\boxed{T_k<\infty\ \text{almost surely},\qquad \mathbb E T_k=\infty.}
$$

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
