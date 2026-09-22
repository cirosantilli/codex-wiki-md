<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Two [absolute values on a field](../../../../../../absolute-value-algebra.md) are [equivalent absolute values](../../../../../../equivalent-absolute-values.md) when they induce the same [topology](../../../../../../topology-split.md). For nontrivial [absolute values on a field](../../../../../../absolute-value-algebra.md) this is equivalent to

$$
|x|_2=|x|_1^c\qquad(x\in K)
$$

for a fixed real number $c>0$. The [trivial absolute value](../../../../../../trivial-absolute-value.md) is equivalent only to itself.

Restriction of a [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md) plainly preserves the [ultrametric inequality](../../../../../../ultrametric-inequality.md). Conversely, if the restriction is non-Archimedean, every integer, interpreted in either [field](../../../../../../field.md), has [absolute value on a field](../../../../../../absolute-value-algebra.md) at most one. In particular every binomial [coefficient](../../../../../../coefficient.md) has [absolute value on a field](../../../../../../absolute-value-algebra.md) at most one. The [triangle inequality](../../../../../../triangle-inequality.md) applied to the binomial expansion gives, for $x,y\in L$ and every positive integer $N$,

$$
|x+y|^N
\leq\sum_{j=0}^N\left|\binom Nj x^j y^{N-j}\right|
\leq (N+1)\max(|x|,|y|)^N.
$$

Raise both sides to the power $1/N$ and let $N\to\infty$. Since $(N+1)^{1/N}\to1$, this yields

$$
\boxed{|x+y|\leq\max(|x|,|y|).}
$$

This is the [bounded-integer criterion for a non-Archimedean absolute value](../../../../../../bounded-integer-criterion-for-a-non-archimedean-absolute-value.md). The proof works for arbitrary [field extensions](../../../../../../field-extension.md), not just algebraic ones, and in positive characteristic as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
