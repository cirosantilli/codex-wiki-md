<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For

$$
E:y^2=x^3+ax+b,
$$

the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md) gives, for distinct nonopposite points $P=(x_1,y_1)$ and $Q=(x_2,y_2)$,

$$
\lambda=\frac{y_2-y_1}{x_2-x_1},
\qquad
x(P+Q)=\lambda^2-x_1-x_2,
\qquad
y(P+Q)=-y_1+\lambda(x_1-x(P+Q)).
$$

For doubling, replace the slope by

$$
\lambda=\frac{3x_1^2+a}{2y_1}.
$$

The point at infinity is the identity and $-(x,y)=(x,-y)$.

Let the $x$-coordinates of $P,Q,P+Q,P-Q$ be $x_1,x_2,x_3,x_4$. Applying the addition formula with $Q$ and $-Q$ gives

$$
x_3+x_4
=\frac{(y_2-y_1)^2+(y_2+y_1)^2}{(x_2-x_1)^2}-2(x_1+x_2).
$$

Substituting $y_i^2=x_i^3+ax_i+b$ and simplifying yields

$$
x_3+x_4
=\frac{2(x_1x_2+a)(x_1+x_2)+4b}{(x_1-x_2)^2}.
$$

Multiplying the two addition formulas and eliminating $y_1y_2$ in the same way gives

$$
x_3x_4
=\frac{(x_1x_2-a)^2-4b(x_1+x_2)}{(x_1-x_2)^2}.
$$

These identities are the algebraic source of two [parallelogram laws](../../../../../../parallelogram-law.md). Applied to pullbacks of the pole divisor of $x$, they imply

$$
\deg(\varphi+\psi)+\deg(\varphi-\psi)
=2\deg\varphi+2\deg\psi
$$

for [isogenies of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md). Together with $\deg(n\varphi)=n^2\deg\varphi$, this makes the degree a [quadratic form](../../../../../../quadratic-form.md). Applied to the [Absolute logarithmic Weil height](../../../../../../absolute-logarithmic-weil-height.md) of the four $x$-coordinates, with bounded terms removed by passage to the limit defining the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md), they similarly give

$$
\boxed{\widehat h(P+Q)+\widehat h(P-Q)
=2\widehat h(P)+2\widehat h(Q),
\qquad
\widehat h(nP)=n^2\widehat h(P).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
