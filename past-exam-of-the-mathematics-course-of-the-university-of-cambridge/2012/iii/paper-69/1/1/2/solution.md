<h1 id="1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

By the [extreme value theorem](../../../../../../../extreme-value-theorem.md), $p_0=\min_{[-1,1]}p$ is strictly positive, and $p,q,r$ are bounded. The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) therefore gives

$$
|a(u,v)|\leq C\|u\|_{H^2}\|v\|_{H^2},\qquad
|\ell(v)|\leq\|f\|_2\|v\|_2\leq\|f\|_2\|v\|_{H^2}.
$$

For completeness, the [clamped interval derivative norm bound](../../../../../../../clamped-interval-derivative-norm-bound.md) follows from $v'(-1)=v(-1)=0$ and the [one-dimensional Sobolev representative](../../../../../../../one-dimensional-sobolev-representative.md): integrate $v''$ to recover $v'$, and then $v'$ to recover $v$. Applying [Cauchy-Schwarz](../../../../../../../cauchy-schwarz-inequality.md) and integrating over an interval of length two gives

$$
\|v'\|_2\leq2\|v''\|_2,\qquad
\|v\|_2\leq2\|v'\|_2\leq4\|v''\|_2.
$$

Consequently $\|v\|_{H^2}^2\leq21\|v''\|_2^2$. Nonnegativity of $q,r$ yields the precise [coercive bilinear form](../../../../../../../coercive-bilinear-form.md) bound

$$
a(v,v)\geq p_0\|v''\|_2^2\geq\frac{p_0}{21}\|v\|_{H^2}^2.
$$

The [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md) states that a bounded bilinear form on a real [Hilbert space](../../../../../../../hilbert-space-split.md) satisfying $a(v,v)\geq c\|v\|^2$ with $c>0$ represents every bounded linear functional uniquely: there is exactly one $u$ with $a(u,v)=\ell(v)$ for all $v$. All of its hypotheses have now been verified on $H$.

This [weak solution](../../../../../../../weak-solution.md) is the unique global minimum, rather than merely a stationary point. The [Ritz-Galerkin equivalence for a symmetric coercive form](../../../../../../../ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md) here is the exact identity

$$
J(u+w)-J(u)=\frac12a(w,w)\geq\frac{p_0}{42}\|w\|_{H^2}^2.
$$

It is strictly positive for every nonzero $w\in H$. Conversely, a minimum has zero first variation in every direction, so it satisfies the same weak equation. Density of compactly supported [test functions](../../../../../../../test-function.md) and boundedness of $a,\ell$ extend the distributional equation back to all $H$ test vectors. **There is exactly one minimum, and it is exactly the clamped weak solution.** No additional coefficient smoothness or classical fourth derivative is needed.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Section I](../../../section-i.md)
5. [Paper 69](../../../../paper-69-split.md)
6. [Iii](../../../../split.md)
7. [2012](../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
