<h1 id="28k/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For every estimator, its worst-case risk dominates its average risk under the [uniform prior](../../../../../../../uniform-prior.md). Since the preceding [Bayes estimator](../../../../../../../bayes-estimator.md) minimizes that average,

$$
\sup_{0<p<1}R(p,\delta)\ge\int_0^1R(p,\delta)\,dp\ge1/n.
$$

The estimator $X/n$ has risk exactly $1/n$ throughout the interior, so it attains this lower bound. Under either endpoint convention discussed above its supremum over $[0,1]$ is also $1/n$. Thus

$$
\boxed{\delta_{\rm minimax}=X/n,\qquad\inf_\delta\sup_pR(p,\delta)=1/n}.
$$

This constant-risk Bayes argument works also for $n=1$, when the only observed counts are endpoints and the posterior integrability argument still selects their corresponding decisions.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [28K](../../../28k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
