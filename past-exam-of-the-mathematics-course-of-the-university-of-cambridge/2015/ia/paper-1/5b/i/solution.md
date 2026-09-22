<h1 id="5b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in $\mathbb R^n$ is

$$
\boxed{|a\cdot b|\leq\|a\|\,\|b\|.}
$$

Here the [Euclidean norm](../../../../../../euclidean-norm.md) is induced by the [dot product](../../../../../../dot-product.md). If $b=0$, the result is immediate. If $b\ne0$, the squared [Euclidean norm](../../../../../../euclidean-norm.md) of the component of $a$ perpendicular to $b$ is nonnegative:

$$
0\leq\left\|a-\frac{a\cdot b}{\|b\|^2}b\right\|^2=\|a\|^2-\frac{(a\cdot b)^2}{\|b\|^2}.
$$

Rearrangement proves the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Equality holds precisely when $a$ and $b$ are linearly dependent, including the cases of a zero vector.

Expanding the squared [Euclidean norm](../../../../../../euclidean-norm.md) and using the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\|a+b\|^2=\|a\|^2+2a\cdot b+\|b\|^2\leq(\|a\|+\|b\|)^2.
$$

Taking nonnegative square roots gives the [triangle inequality](../../../../../../triangle-inequality.md). Applying the [triangle inequality](../../../../../../triangle-inequality.md) once more gives

$$
\boxed{\|a+b\|\leq\|a\|+\|b\|,\qquad\|a+b+c\|\leq\|a\|+\|b\|+\|c\|.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5B](../../5b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
