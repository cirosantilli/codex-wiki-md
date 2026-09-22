<h1 id="24i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a point $Q\in E$. Since $g(E)=1$, a nonzero regular differential has an effective divisor of degree $2g-2=0$, so $K_E\sim0$. The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) therefore gives

$$
\ell(nQ)=n\qquad(n\geq1).
$$

Choose

$$
x\in L(2Q)\setminus L(Q),
\qquad
y\in L(3Q)\setminus L(2Q).
$$

The [rational functions](../../../../../../rational-function.md) $x$ and $y$ have their only poles at $Q$, of orders two and three respectively.

The seven functions

$$
1,x,y,x^2,xy,x^3,y^2
$$

belong to the six-dimensional [Riemann-Roch space](../../../../../../riemann-roch-space.md) $L(6Q)$, so they satisfy a nontrivial linear relation. Comparing pole orders shows that the coefficients of both $x^3$ and $y^2$ are nonzero. After rescaling, the relation has the [Weierstrass form](../../../../../../weierstrass-equation-of-an-elliptic-curve.md)

$$
y^2+a_1xy+a_3y=x^3+a_2x^2+a_4x+a_6.
$$

The divisor $3Q$ is [very ample](../../../../../../very-ample-divisor.md), so its complete linear system embeds $E$ in $\mathbb P^2$ and the displayed relation cuts out its image; this is the [Weierstrass construction from Riemann-Roch in genus one](../../../../../../weierstrass-construction-from-riemann-roch-in-genus-one.md).

Because $\operatorname{char}k\ne2$, completing the square removes the terms linear in $y$, and because $\operatorname{char}k\ne3$, translating $x$ removes the quadratic term. Thus the equation becomes

$$
y^2=x^3+Ax+B.
$$

Since $k$ is [algebraically closed](../../../../../../algebraically-closed-field.md), the cubic factors as

$$
x^3+Ax+B=(x-\lambda_1)(x-\lambda_2)(x-\lambda_3).
$$

Smoothness of $E$ says that the [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) is nonzero, equivalently the three roots are distinct. Hence

$$
\boxed{E\cong\{y^2=(x-\lambda_1)(x-\lambda_2)(x-\lambda_3)\}\subset\mathbb P^2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24I](../../24i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
