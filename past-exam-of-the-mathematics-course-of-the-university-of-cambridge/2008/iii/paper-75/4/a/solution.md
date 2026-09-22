<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [function](../../../../../../function-split.md) on an interval, the [modulus of continuity](../../../../../../modulus-of-continuity.md) is $\omega(f,t)=\sup_{|x-y|\le t}|f(x)-f(y)|$, with the pair restricted to that interval. For a periodic [function](../../../../../../function-split.md) the equivalent definition is $\sup_{\theta,|h|\le t}|g(\theta+h)-g(\theta)|$. The [mean value theorem](../../../../../../mean-value-theorem.md) and $|\sin\theta|\le1$ give

$$
|\cos(\theta+h)-\cos\theta|\le|h|.
$$

Both cosine values lie in $[-1,1]$. Hence for $|h|\le t$,

$$
|\widetilde f(\theta+h)-\widetilde f(\theta)|
=|f(\cos(\theta+h))-f(\cos\theta)|\le\omega(f,t).
$$

Taking the supremum proves

$$
\boxed{\omega(\widetilde f,t)\le\omega(f,t).}
$$

If the periodic [modulus of continuity](../../../../../../modulus-of-continuity.md) is defined using circular distance instead, choose lifts at that shortest distance and apply the same argument. The [cosine substitution for polynomial approximation](../../../../../../cosine-substitution-for-polynomial-approximation.md) therefore does not enlarge this modulus.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
