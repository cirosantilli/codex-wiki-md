<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the [scale family](../../../../../../scale-family.md) has the differentiability needed for [Fisher information](../../../../../../fisher-information-matrix.md), and the following constant is finite and positive. With $\ell_f(u)=\log f(u)$, the [score function](../../../../../../informant-function.md) is

$$
\partial_\sigma\log p(y\mid\sigma)
=-\frac{1+u\ell_f'(u)}{\sigma},\qquad u=y/\sigma.
$$

Part (b) therefore gives

$$
I(\sigma)=\frac C{\sigma^2},\qquad
C=\int[1+u\ell_f'(u)]^2f(u)\,du,
$$

where $C$ is independent of $\sigma$. The [Jeffreys prior for a scale parameter](../../../../../../jeffreys-prior-for-a-scale-parameter.md) is consequently

$$
\boxed{p_J(\sigma)\propto\sigma^{-1},\qquad\sigma>0.}
$$

The reciprocal-of-a-reciprocal in the TeX is a transcription error; the PDF has $\sigma^{-1}$. The expected-Hessian information identity should not be applied indiscriminately to nonregular parameter-dependent supports.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
