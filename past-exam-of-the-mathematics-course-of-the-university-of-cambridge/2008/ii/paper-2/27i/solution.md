<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

Interpret $\phi(x)$ as the conditional rejection probability. The [Type I error](../../../../../type-i-and-type-ii-errors.md) is $\alpha=E_0\phi(X)$, the [Type II error](../../../../../type-i-and-type-ii-errors.md) is $\beta=E_1[1-\phi(X)]$, the size is $\alpha$, and the power is $1-\beta$. Their weighted sum is

$$
c\alpha+\beta=1+\int\phi(x)[cp_0(x)-p_1(x)]dx.
$$

Pointwise minimization over $0\le\phi\le1$ forces rejection where $p_1>cp_0$ and acceptance where $p_1<cp_0$, with arbitrary randomization on equality. Conversely those choices minimize every integrand. The equivalence holds almost everywhere, since changing a test on a common null set cannot change its errors. With both weights strictly positive, any simultaneous improvement of the two errors, strict in at least one, would lower this weighted sum. **Every such positive-threshold [likelihood ratio](../../../../../likelihood-ratio.md) test is admissible for the two simple hypotheses.**

For the specified densities the [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
R_\theta(x)=\begin{cases}0,&0<x<\theta,\\\dfrac{x-\theta}{x(1-\theta)^2},&\theta\le x\le1.\end{cases}
$$

It increases strictly on $(\theta,1)$ from zero to $1/(1-\theta)$. For $0<c<1/(1-\theta)$, the [likelihood-ratio test](../../../../../likelihood-ratio-test.md) rejects when $x>\theta/[1-c(1-\theta)^2]$. Larger thresholds accept almost surely. Threshold zero rejects everywhere above $\theta$ and permits arbitrary rejection below $\theta$, where both weighted choices tie; values at individual endpoints do not affect errors. These describe all nonnegative-threshold [likelihood ratio](../../../../../likelihood-ratio.md) tests, including their limiting accept-all and reject-all cases.

The upper-tail test $\phi_k$ has size $1-k^2$. If $\theta<k$, it is a positive-threshold [likelihood ratio](../../../../../likelihood-ratio.md) test and is admissible. If $\theta=k$, it rejects exactly the alternative's support, with power one; no test can retain power one with smaller size, so it remains admissible. If $\theta>k$, it still has power one but wastes rejection probability on $(k,\theta)$, where the alternative density vanishes. The test $\phi_\theta$ has the same power and smaller size, so

$$
\boxed{\phi_k\text{ is admissible against fixed }\theta\iff\theta\le k.}
$$

Nevertheless $\phi_k$ is a [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) at size $1-k^2$ against all $0<\theta<1$: for $\theta<k$, apply the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md); for $\theta\ge k$, its power is already the maximum one. It is also admissible against the composite alternative. Indeed choose any $0<\theta<k$. Strict monotonicity of its [likelihood ratio](../../../../../likelihood-ratio.md) makes $\phi_k$ the unique positive-threshold minimizer up to null sets. A test dominating it for the composite problem would either improve the weighted simple risk at this $\theta$, impossible, or tie that risk and coincide almost everywhere. Since $p_0>0$ throughout $(0,1)$, such coincidence also precludes improvement at any other $\theta$.

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
