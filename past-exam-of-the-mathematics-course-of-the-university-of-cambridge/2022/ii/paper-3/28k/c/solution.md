<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\sqrt n(\overline X_n-\mu)\xrightarrow{d}N(0,1).
$$

Applying the [delta method](../../../../../../delta-method.md) to $g(x)=x^2$ yields

$$
\boxed{
\sqrt n(T_n-\mu^2)
\xrightarrow{d}N(0,4\mu^2)
}.
$$

For $\mu=0$ this denotes the degenerate distribution at zero, which is the correct limit at the $\sqrt n$ scale.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
