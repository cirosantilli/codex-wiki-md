<h1 id="16b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since every [eigenvalue](../../../../../../eigenvalue.md) has modulus less than one, $1$ is not an [eigenvalue](../../../../../../eigenvalue.md) and $I-H$ is invertible. Hence the iteration has a unique [fixed point](../../../../../../fixed-point.md) $\widehat x=(I-H)^{-1}v$. The stated consistency implication gives $A\widehat x=b$, and nonsingularity of $A$ identifies $\widehat x=x^*$. This justifies using the fixed-point relation even though consistency was stated in only one direction.

Expand the initial error in the eigenvector [basis](../../../../../../basis.md), $x^0-x^*=\sum_i c_iw_i$. Subtract the fixed-point equation from the [stationary iterative method for a linear system](../../../../../../stationary-iterative-method-for-a-linear-system.md) and iterate:

$$
x^k-x^*=H^k(x^0-x^*)=\sum_{i=1}^n c_i\lambda_i^k w_i.
$$

With $q=\max_i|\lambda_i|<1$, any [norm](../../../../../../norm.md) obeys $\|x^k-x^*\|\le q^k\sum_i|c_i|\|w_i\|\to0$. Thus

$$
\boxed{x^k\longrightarrow x^*\quad\text{for every initial vector}}.
$$

The argument uses the given diagonalizable eigenbasis; the more general convergence criterion is [spectral radius](../../../../../../spectral-radius.md) less than one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
