<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $m$ be the [multiplicity](../../../../../../multiplicity-mathematics.md) at zero, and write $f(z)=z^m h(z)$ with $h(0)\ne0$. The proof in [solution](../a/solution.md) gives $|f|\le1$. For radii without boundary zeros, [Jensen's formula](../../../../../../jensen-s-formula.md) says

$$
\int\log|f(re^{i\theta})|\,dm
=m\log r+\log|h(0)|+\sum_{0<|a_n|<r}\log\frac r{|a_n|}.
$$

The absolute logarithmic hypothesis makes the left side tend to zero. The nonnegative zero sum increases to $\sum_n\log(1/|a_n|)$ by the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), so this series is finite. Hence $\sum_n(1-|a_n|)<\infty$, and the [Blaschke condition](../../../../../../blaschke-condition.md) supplies a [Blaschke product](../../../../../../blaschke-product.md) $B$ with exactly these zeros and their [multiplicities](../../../../../../multiplicity-mathematics.md).

The quotient $g=f/B$ extends [holomorphically](../../../../../../holomorphic-function.md) across every zero because the [multiplicities](../../../../../../multiplicity-mathematics.md) agree, and the extensions have nonzero values. Thus **$f=Bg$ with $g$ zero-free and holomorphic**. We will also need the stronger [Blaschke factorization of a bounded holomorphic function](../../../../../../blaschke-factorization-of-a-bounded-holomorphic-function.md), namely $|g|\le1$. Let $B_N$ contain the factor $z^m$ and the first $N$ other zero factors. The quotient $f/B_N$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md). On $|z|=R$ enclosing those finitely many zeros, its modulus is at most $1/\min_{|z|=R}|B_N(z)|$. The [maximum modulus principle](../../../../../../maximum-modulus-principle.md) transfers this bound to the interior. Since the finite [Blaschke product](../../../../../../blaschke-product.md) has boundary modulus one continuously, letting $R\uparrow1$ gives $|f/B_N|\le1$. Now let $N\to\infty$ using [locally uniform convergence](../../../../../../locally-uniform-convergence.md) of the [Blaschke product](../../../../../../blaschke-product.md), first off the zeros and then by [continuity](../../../../../../continuous-function.md) at them. This proves $|g|\le1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
