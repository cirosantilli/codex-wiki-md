<h1 id="10g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For any vector $y\in\mathbb F_2^n$, use its [Hamming weight](../../../../../../hamming-weight.md) $w(y)=\#\{j:y_j=1\}$. The stated product identity also follows directly by summing each coordinate independently:

$$
\sum_y u^{w(y)}(-1)^{x\cdot y}
=\prod_{j=1}^n(1+(-1)^{x_j}u)
=(1-u)^{w(x)}(1+u)^{n-w(x)}.
$$

For $t\ne0$, interchange the two finite sums with $u=s/t$. [Character orthogonality](../../../../../../character-orthogonality.md) evaluates the inner sum over codewords, whereas the product identity evaluates the sum over all binary vectors. Thus

$$
2^k\sum_{y\in C^\perp}(s/t)^{w(y)}
=\sum_{x\in C}(1-s/t)^{w(x)}(1+s/t)^{n-w(x)}.
$$

Multiply by $t^n$ to obtain the [MacWilliams identity](../../../../../../macwilliams-identity.md) in the paper's weight-enumerator convention:

$$
\boxed{W_{C^\perp}(s,t)=2^{-k}W_C(t-s,t+s)}.
$$

Both sides are [polynomials](../../../../../../polynomial-split.md), so equality for $t\ne0$ extends to $t=0$ as well; the intermediate quotient is not a restriction on the final identity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10G](../../10g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
