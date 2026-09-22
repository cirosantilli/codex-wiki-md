<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The two cosets of $2\mathbb Z_2$ are [clopen sets](../../../../../../clopen-set.md) in the [2-adic integers](../../../../../../2-adic-integer.md). The function is constant on each, so it is a [locally constant function](../../../../../../locally-constant-function.md) and therefore [continuous](../../../../../../continuous-function.md). Its values on the nonnegative integers are $f(j)=(-1)^j$.

The [Mahler coefficient](../../../../../../mahler-coefficient.md) at index $n$ is the nth [forward difference operator](../../../../../../forward-difference-operator.md) applied at zero. Here

$$
a_n=\sum_{j=0}^n(-1)^{n-j}\binom nj(-1)^j=(-1)^n\sum_{j=0}^n\binom nj=(-2)^n.
$$

Thus the [Mahler expansion of the parity function](../../../../../../mahler-expansion-of-the-parity-function.md) is

$$
\boxed{f(x)=\sum_{n=0}^{\infty}(-2)^n\binom xn,\qquad x\in\mathbb Z_2.}
$$

To verify the expansion directly, each [binomial polynomial](../../../../../../binomial-polynomial.md) $\binom xn$ takes values in $\mathbb Z_2$: it does so at nonnegative integers, which form a [dense subset](../../../../../../dense-set.md), and polynomial evaluation is [continuous](../../../../../../continuous-function.md) into $\mathbb Q_2$. Hence the nth summand has [2-adic absolute value](../../../../../../2-adic-absolute-value.md) at most $2^{-n}$ throughout the domain. The [ultrametric inequality](../../../../../../ultrametric-inequality.md) proves [uniform convergence](../../../../../../uniform-convergence.md), and the sum is [continuous](../../../../../../continuous-function.md). At each nonnegative integer $m$, the series becomes the finite [binomial theorem](../../../../../../binomial-theorem.md) identity $(1-2)^m=(-1)^m$. Equality on a [dense subset](../../../../../../dense-set.md) and [continuity](../../../../../../continuous-function.md) prove equality everywhere. Finally, the coefficients in any such expansion are determined successively by its values at $0,1,2,\ldots$, since $\binom mn=0$ for $n>m$ and $\binom mm=1$. This also verifies uniqueness without needing the general [Mahler theorem](../../../../../../mahler-s-theorem.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
