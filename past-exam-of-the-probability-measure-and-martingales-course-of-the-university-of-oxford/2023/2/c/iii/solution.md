<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose $Z_\infty$ as the pointwise [limit of a sequence](../../../../../limit-of-a-sequence.md) of $(Z_n)$ where it exists, and as zero otherwise. The convergence [event](../../../../../event.md) and every $Z_n$ are $\sigma(X)$-[measurable](../../../../../measurability.md), so this is an exactly $\sigma(X)$-[measurable](../../../../../measurability.md) version, bounded by $L$. Part (a)(ii), the [Doob-Dynkin lemma](../../../../../doob-dynkin-lemma.md), supplies a [Borel measurable function](../../../../../borel-measurable-function.md) $g$ on $[0,1]$ such that $Z_\infty=g(X)$. Applying [scalar clipping](../../../../../scalar-clipping.md) to $g$ with bounds $[-L,L]$ preserves that equality and ensures $|g(u)|\leq L$ everywhere.

Part (c)(ii) and the [conditional expectation](../../../../../conditional-expectation.md) formula from part (b)(iv) now give

$$
\boxed{Z_n=\mathbb E[g(X)\mid\mathcal F_n]
=2^n\int_{X_n}^{X_n+2^{-n}}g(u)\,du\quad\text{almost surely}.}
$$

Since the indices $n$ form a [countable](../../../../../countable-set.md) family, these identities may be taken on one common full-[probability](../../../../../probability.md) [event](../../../../../event.md).

For fixed $n,k$, both the slope and the displayed average are constant on the atom $A_{n,k}$, whose [probability](../../../../../probability.md) is $2^{-n}>0$. An equality holding [almost surely](../../../../../almost-sure-convergence.md) of these constants forces the deterministic equality

$$
f((k+1)2^{-n})-f(k2^{-n})
=\int_{k2^{-n}}^{(k+1)2^{-n}}g(u)\,du.
$$

Sum over $0\leq k<j$. The [telescoping sum](../../../../../telescoping-sum.md) gives

$$
f(j2^{-n})-f(0)=\int_0^{j2^{-n}}g(u)\,du,
\qquad 0\leq j\leq2^n.
$$

Thus the desired identity holds at every dyadic endpoint, including $1$, without evaluating the undefined slope at $X=1$.

Finally, given $x\in[0,1]$, take dyadic endpoints $x_n\to x$. The [Lipschitz condition](../../../../../lipschitz-continuity.md) implies $|f(x_n)-f(x)|\leq L|x_n-x|$, and the bound on the [Borel measurable function](../../../../../borel-measurable-function.md) $g$ gives

$$
\left|\int_0^{x_n}g(u)\,du-\int_0^xg(u)\,du\right|\leq L|x_n-x|.
$$

Passing to the [limit of a sequence](../../../../../limit-of-a-sequence.md) proves

$$
\boxed{f(x)-f(0)=\int_0^xg(u)\,du\quad\text{for every }x\in[0,1].}
$$

This is a [martingale proof of the integral representation of a Lipschitz function](../../../../../martingale-proof-of-the-integral-representation-of-a-lipschitz-function.md). It constructs a bounded [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md) representing the increments of $f$, and in particular proves [absolute continuity](../../../../../absolutely-continuous-function.md) of $f$. No prior assumption that $f$ has a [derivative](../../../../../derivative.md) is needed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
