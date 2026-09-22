<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Outside the [countable set](../../../../../../countable-set.md) of dyadic rational numbers, the [binary expansion](../../../../../../binary-expansion.md) $x=\sum_{j\geq1}\epsilon_j(x)2^{-j}$ is unique. Multiplication by two modulo one deletes the first binary digit, so

$$
\epsilon_j(x)=\mathbf1_{[1/2,1)}(E_2^{j-1}x).
$$

Let $g=\mathbf1_{[1/2,1)}$. By part (b), the [doubling map](../../../../../../dyadic-transformation.md) is a [measure-preserving transformation](../../../../../../measure-preserving-transformation.md) and is [ergodic](../../../../../../ergodicity.md) for [Lebesgue measure](../../../../../../lebesgue-measure.md). Applying the [Birkhoff ergodic theorem](../../../../../../birkhoff-ergodic-theorem.md) to this [indicator function](../../../../../../indicator-function.md) gives

$$
\frac1n\#\{1\leq j\leq n:\epsilon_j(x)=1\}
=\frac1n\sum_{k=0}^{n-1}g(E_2^kx)
\longrightarrow\int_0^1g(x)\,dx=\frac12
$$

for almost every $x$. The dyadic rationals have [Lebesgue measure](../../../../../../lebesgue-measure.md) zero, so the choice of their two possible [binary expansions](../../../../../../binary-expansion.md) does not affect the conclusion. Thus **the limiting frequency of the digit one is $1/2$ almost everywhere**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
