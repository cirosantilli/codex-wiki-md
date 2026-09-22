<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $u=x_1-1$, $v=y_1$. Then $v^2=u(u^2+3u+2)$. After using the curve equation, the displayed rational functions become

$$
X=x_1+\frac2{x_1-1}=u+1+\frac2u,\qquad
Y=v\left(1-\frac2{u^2}\right).
$$

Set $X_0=X+2=u+3+2/u$. Direct substitution into $v^2=u(u^2+3u+2)$ gives

$$
Y^2=X_0(X_0^2-6X_0+1)=X_0^3-X_0^2+X_0
$$

over $\mathbb F_5$. Replacing $X_0$ by $X+2$ makes this $Y^2=X^3-X+1$. This verifies the target equation explicitly, and identifies the functions with the [two-isogeny formula](../../../../../../two-isogeny-formula.md) after translating the source's two-torsion point to zero and then translating the target coordinate.

We must also check the omitted affine points. At $T=(1,0)$, $v$ is a [local parameter](../../../../../../local-parameter-on-a-smooth-algebraic-curve.md), and $u=v^2/(x_1(x_1+1))$ has order two, since $x_1(x_1+1)=2$ at $T$. Thus $X$ has a pole of order two and $Y$ one of order three. At $O_1$, the usual [pole orders on a smooth cubic in Weierstrass form](../../../../../../pole-orders-on-a-smooth-cubic-in-weierstrass-form.md) give poles two and three as well: the correction terms have higher order and do not cancel their leading terms. There are no other poles. A rational map from a smooth curve into a projective curve extends across these points; the indicated pole orders show that both $T$ and $O_1$ map to $O_2$. Hence this is a nonconstant identity-preserving morphism, and part (i) makes it an [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md).

The pullback of the pole divisor $2O_2$ of $X$ is $2O_1+2T$. Degrees of divisors multiply by the morphism degree, so $2\deg\varphi=4$. We obtain

$$
\boxed{\deg\varphi=2,\qquad\ker\varphi=\{O_1,(1,0)\}.}
$$

The degree is [prime](../../../../../../prime-number.md) to five, so the [elliptic isogeny](../../../../../../isogeny-of-elliptic-curves.md) is separable. Equivalently $dX/Y=dx_1/y_1$ is a nonzero pullback of an invariant differential.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
