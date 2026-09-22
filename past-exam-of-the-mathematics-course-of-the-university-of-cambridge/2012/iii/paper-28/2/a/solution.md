<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A useful version is the [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md). Let $K$ be complete for a [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md), let $f\in\mathcal O_K[X]$, and suppose $a\in\mathcal O_K$ satisfies

$$
|f(a)|<|f'(a)|^2.
$$

Then there is a unique root $\alpha$ in the ball $|\alpha-a|<|f'(a)|$, and $|\alpha-a|\leq|f(a)/f'(a)|$.

Put $h=|f'(a)|$ and $\eta=|f(a)|/h^2<1$. Starting with $x_0=a$, apply [Newton iteration over a valued field](../../../../../../newton-iteration-over-a-valued-field.md) $x_{n+1}=x_n-f(x_n)/f'(x_n)$. Taylor expansion over the [valuation ring](../../../../../../valuation-ring.md) gives

$$
|f(x+u)-f(x)-f'(x)u|\leq|u|^2,\qquad |f'(x+u)-f'(x)|\leq|u|
$$

for integral $x,u$. Inductively $|f'(x_n)|=h$ and $|f(x_n)|/h^2\leq\eta^{2^n}$. Indeed the Newton increment has size at most $h\eta^{2^n}<h$, so the derivative size is unchanged, and the new function value is bounded by the square of the increment. The increments tend to zero, and the ultrametric inequality makes the sequence Cauchy. Completeness supplies a root with the stated distance bound.

If $b,c$ are distinct points of the ball, their divided difference is $f'(a)$ plus a term of size at most $\max(|b-a|,|c-a|)<h$, so $(f(b)-f(c))/(b-c)$ is nonzero. Two roots in that ball are impossible. **This proves the stated [Hensel lemma](../../../../../../hensel-s-lemma.md).** In particular a simple root modulo the [maximal ideal](../../../../../../maximal-ideal.md) lifts uniquely to a root in its residue class.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
