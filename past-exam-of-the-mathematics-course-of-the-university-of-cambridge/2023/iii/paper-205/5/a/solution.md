<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the normalization used in the question, [ridge regression](../../../../../../ridge-regression.md) solves

$$
\min_{\mu\in\mathbb R,\,\beta\in\mathbb R^p}
\bigl\|Y-\mu\mathbf1-X\beta\bigr\|_2^2+\lambda\|\beta\|_2^2.
$$

Differentiating with respect to $\mu$ and using the centered columns $X^T\mathbf1=0$ gives $\widehat\mu=\overline Y$. The [normal equation](../../../../../../normal-equation.md) for $\beta$ is

$$
(X^TX+\lambda I)\widehat\beta=X^TY,
$$

so

$$
\widehat\beta=(X^TX+\lambda I)^{-1}X^TY.
$$

The [push-through identity](../../../../../../push-through-identity.md) then gives the equivalent dual form

$$
\boxed{\widehat\beta=X^T(XX^T+\lambda I)^{-1}Y.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
