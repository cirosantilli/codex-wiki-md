<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho$ afford the [character](../../../../character-of-a-representation.md) $\chi$, and let $m$ be the [order of a group element](../../../../order-of-a-group-element.md) $g$. Then $\rho(g)^m=I$, so its [minimal polynomial](../../../../minimal-polynomial.md) divides $T^m-1$. Over the [complex numbers](../../../../complex-number.md) this [polynomial](../../../../polynomial-split.md) has distinct [polynomial roots](../../../../root-of-a-polynomial.md), since its [formal derivative](../../../../formal-derivative.md) $mT^{m-1}$ does not vanish at any of its [polynomial roots](../../../../root-of-a-polynomial.md). Thus $\rho(g)$ is [diagonalizable](../../../../diagonalizable-matrix.md), with [eigenvalues](../../../../eigenvalue.md) $\lambda_1,\ldots,\lambda_d$ that are [roots of unity](../../../../root-of-unity.md).

Each $\lambda_j$ has [absolute value](../../../../absolute-value.md) one, so $\lambda_j^{-1}=\overline{\lambda_j}$. The [eigenvalues](../../../../eigenvalue.md) of $\rho(g^{-1})=\rho(g)^{-1}$ are $\lambda_j^{-1}$, giving

$$
\boxed{\chi(g^{-1})=\sum_j\lambda_j^{-1}
=\sum_j\overline{\lambda_j}
=\overline{\chi(g)}.}
$$

This is the [character inversion identity](../../../../character-inversion-identity.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
