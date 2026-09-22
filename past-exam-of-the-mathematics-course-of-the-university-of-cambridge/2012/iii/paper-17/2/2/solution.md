<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the [differential one-form](../../../../../../one-form.md) as $\omega=\sum_i\omega_i\,dx^i$, and the [vector fields](../../../../../../vector-field.md) as $X=X^i\partial_i$, $Y=Y^i\partial_i$. The coordinate definition of the [exterior derivative](../../../../../../exterior-derivative.md) gives

$$
d\omega(X,Y)=\sum_{i,j}(\partial_i\omega_j-\partial_j\omega_i)X^iY^j.
$$

Expand the right side of the invariant formula:

$$
\begin{aligned}
X(\omega(Y))-Y(\omega(X))
={}&\sum_{i,j}(\partial_i\omega_j)X^iY^j
-\sum_{i,j}(\partial_i\omega_j)Y^iX^j\\
&+\sum_{i,j}\omega_j(X^i\partial_iY^j-Y^i\partial_iX^j).
\end{aligned}
$$

The last line is $\omega([X,Y])$, by the coordinate formula for the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md). Subtract it and interchange the two indices in the second sum. The remaining terms are exactly $d\omega(X,Y)$. Therefore

$$
\boxed{d\omega(X,Y)=X(\omega(Y))-Y(\omega(X))-\omega([X,Y]).}
$$

This is the [exterior derivative of a one-form evaluated on vector fields](../../../../../../exterior-derivative-of-a-one-form-evaluated-on-vector-fields.md); it is valid in any frame, not just a commuting coordinate frame.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
