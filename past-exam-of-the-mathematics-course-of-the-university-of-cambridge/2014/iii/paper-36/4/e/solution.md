<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

At a common proposal budget, the two asymptotic variances are

$$
v_{\rm IS}=\int\phi^2\frac{f^2}{g}-\theta^2,\qquad v_{\rm rej}=M\left(\int\phi^2f-\theta^2\right).
$$

Thus **prefer the estimator with the smaller proposal-budget [variance](../../../../../../variance-split.md); the stated assumptions do not give a universal winner**. [Importance sampling](../../../../../../importance-sampling.md) uses every proposal and avoids an empty accepted sample, but those facts alone do not establish [variance](../../../../../../variance-split.md) dominance. The bound from part (a) only says $v_{\rm IS}\leq Mv_f+(M-1)\theta^2$. If $\theta=0$, it does imply that [importance sampling](../../../../../../importance-sampling.md) is at least as efficient asymptotically.

For explicit nonconstant counterexamples in both directions, take $g(x)=1$ and $f(x)=2x$ on $0<x<1$, and zero outside, with the sharp envelope $M=2$. For $\phi(x)=x$, direct integration gives $\theta=2/3$, $v_f=1/18$ and

$$
\boxed{v_{\rm IS}=16/45>1/9=v_{\rm rej}.}
$$

The accepted-sample mean is better. For the same densities but $\phi(x)=x-1$, the target [variance](../../../../../../variance-split.md) is unchanged, while $\theta=-1/3$ and

$$
\boxed{v_{\rm IS}=1/45<1/9=v_{\rm rej}.}
$$

[Importance sampling](../../../../../../importance-sampling.md) is now better. This is the [variance reversal under additive shifts of an importance-sampling integrand](../../../../../../variance-reversal-under-additive-shifts-of-an-importance-sampling-integrand.md).

There is a useful distinction about the [Rao-Blackwell theorem](../../../../../../rao-blackwell-theorem.md). The weighted importance estimator is the conditional expectation, given the proposals, of the fixed-denominator rejection estimator $(M/n)\sum_i I_i\phi(X_i)$. It is not the conditional expectation of the random-denominator mean $N^{-1}\sum_i I_i\phi(X_i)$. Rao-Blackwell [variance](../../../../../../variance-split.md) reduction for the former therefore does not prove a comparison with the latter. This is the [Rao-Blackwell identity for a fixed-denominator rejection estimator](../../../../../../rao-blackwell-identity-for-a-fixed-denominator-rejection-estimator.md). The appropriate answer is the [proposal-budget variance comparison of importance and rejection sampling](../../../../../../proposal-budget-variance-comparison-of-importance-and-rejection-sampling.md), with the empty-output convention specified.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
