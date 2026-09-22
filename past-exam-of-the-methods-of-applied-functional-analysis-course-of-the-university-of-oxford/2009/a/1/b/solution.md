<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Weak convergence](../../../../../weak-convergence.md) $u_j\rightharpoonup u$ means $F(u_j)\to F(u)$ for every $F\in X^*$. [Weak-star convergence](../../../../../weak-star-topology.md) $T_j\overset*\rightharpoonup T$ means $T_j(x)\to T(x)$ for every $x\in X$, viewing $X$ as the predual. The [Sequential Banach-Alaoglu theorem for a separable predual](../../../../../sequential-banach-alaoglu-theorem-for-a-separable-predual.md) says that every norm-bounded [sequence](../../../../../sequence.md) in $X^*$ has a [weak-star convergent](../../../../../weak-star-topology.md) [subsequence](../../../../../subsequence.md). Separability is what turns the [bounded](../../../../../boundedness.md) [weak-star](../../../../../weak-star-topology.md) [compactness](../../../../../compact-space.md) statement into this sequential form.

For the [weak-star limit of periodic rescalings](../../../../../weak-star-limit-of-periodic-rescalings.md), apply it with $X=L^1(\mathbb R)$, which is separable, and $X^*=L^\infty(\mathbb R)$. The rescaled [functions](../../../../../function-split.md) have uniform [essential-supremum](../../../../../essential-supremum.md) bound $\|\theta\|_\infty$. Let $q=\theta-\bar\theta$ and $F(t)=\int_0^tq(s)\,ds$. Since $q$ is one-periodic with zero mean, $F$ is a [bounded](../../../../../boundedness.md) one-periodic absolutely [continuous](../../../../../continuous-function.md) primitive. Thus for every finite [interval](../../../../../interval-mathematics.md),

$$
\int_a^b[\theta(jx)-\bar\theta],dx=\frac{F(jb)-F(ja)}j\longrightarrow0.
$$

Every [weak-star subsequential limit](../../../../../weak-star-topology.md) $h$ therefore satisfies $\int_a^b(h-\bar\theta)=0$ for all $a<b$. To apply the supplied uniqueness fact without assuming global integrability, fix $R>0$ and [set](../../../../../set-split.md) $v=(h-\bar\theta)\mathbf1_{[-R,R]}$. This is in $L^1(\mathbb R)$, and its [integral](../../../../../integral-split.md) over any [interval](../../../../../interval-mathematics.md) is zero, since intersecting with $[-R,R]$ again gives an [interval](../../../../../interval-mathematics.md). Hence $v=0$ [almost everywhere](../../../../../almost-everywhere.md). Taking integer $R\to\infty$ yields $h=\bar\theta$ [almost everywhere](../../../../../almost-everywhere.md) on the whole line.

Finally, if the full [sequence](../../../../../sequence.md) did not converge [weak-star](../../../../../weak-star-topology.md) to this constant, some $g\in L^1$ and some [subsequence](../../../../../subsequence.md) would have its pairing with $\theta(jx)-\bar\theta$ [bounded](../../../../../boundedness.md) away from zero. Sequential [compactness](../../../../../compact-space.md) gives a further [weak-star convergent](../../../../../weak-star-topology.md) [subsequence](../../../../../subsequence.md), whose [limit](../../../../../limit-of-a-function.md) must be the constant just identified, a contradiction. Therefore

$$
\boxed{\theta(j\cdot)\overset*\rightharpoonup\bar\theta\quad\text{in }L^\infty(\mathbb R).}
$$

This is averaging against integrable [test functions](../../../../../test-function.md), not a claim of [pointwise](../../../../../pointwise-convergence.md) or strong [norm convergence](../../../../../norm-convergence.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
