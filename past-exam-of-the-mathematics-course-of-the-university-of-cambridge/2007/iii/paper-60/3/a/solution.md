<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $A$ is a [bounded operator](../../../../../../continuous-linear-operator.md), its exponential [power series](../../../../../../power-series.md) converges in [operator norm](../../../../../../operator-norm.md). The identity $A^2=I$ gives $A^{2k}=I$ and $A^{2k+1}=A$. Separating the even and odd powers therefore gives

$$
e^{-i\theta A}=\sum_{k=0}^\infty\frac{(-1)^k\theta^{2k}}{(2k)!}I-i\sum_{k=0}^\infty\frac{(-1)^k\theta^{2k+1}}{(2k+1)!}A=\boxed{\cos\theta\,I-i\sin\theta\,A.}
$$

The algebraic identity does not require $A$ to be Hermitian. Hermiticity is additionally needed for this exponential to be a [unitary operator](../../../../../../unitary-operator.md) for real $\theta$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
