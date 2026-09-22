<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a periodic function use the [modulus of continuity](../../../../../../modulus-of-continuity.md)

$$
\omega(g,\delta)=\sup_{\theta\in\mathbb R,\ |h|\le\delta}
|g(\theta+h)-g(\theta)|.
$$

On the interval, take the supremum over pairs of points whose distance is at most $\delta$. The [mean value theorem](../../../../../../mean-value-theorem.md) applied to cosine, whose derivative has absolute value at most one, gives

$$
|\cos(\theta+h)-\cos\theta|\le|h|.
$$

Both cosine values lie in $[-1,1]$, so for $|h|\le\delta$,

$$
|\widetilde f(\theta+h)-\widetilde f(\theta)|
=|f(\cos(\theta+h))-f(\cos\theta)|
\le\omega(f,\delta).
$$

Taking the supremum proves

$$
\boxed{\omega(\widetilde f,\delta)\le\omega(f,\delta)}.
$$

The [cosine substitution for polynomial approximation](../../../../../../cosine-substitution-for-polynomial-approximation.md) is also a linear isometry in the [supremum norm](../../../../../../supremum-norm.md), since cosine maps a full period onto $[-1,1]$; its image consists of even continuous periodic functions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
