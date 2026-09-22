<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a smooth [function](../../../../../../function-split.md), [pullback of a smooth function](../../../../../../pullback-of-a-smooth-function.md) is composition. The [chain rule](../../../../../../chain-rule.md) gives

$$
\boxed{\mathcal L_Xf=\left.\frac{d}{ds}\right|_0f(\phi_s(p))=X(f).}
$$

For a [vector field](../../../../../../vector-field.md) $Y$, use any local coordinates. To first order,

$$
\phi_s^\mu(x)=x^\mu+sX^\mu(x)+O(s^2),\qquad
(d\phi_s)^{-1\mu}{}_{\nu}=\delta^\mu{}_{\nu}-s\partial_\nu X^\mu+O(s^2).
$$

Multiplying this inverse differential by $Y(\phi_s(x))$ gives

$$
(\phi_s^*Y)^\mu=Y^\mu+s\bigl(X^\nu\partial_\nu Y^\mu-Y^\nu\partial_\nu X^\mu\bigr)+O(s^2).
$$

Thus

$$
\boxed{\mathcal L_XY=[X,Y],\qquad
[X,Y]^\mu=X^\nu\partial_\nu Y^\mu-Y^\nu\partial_\nu X^\mu.}
$$

This is the [Lie bracket of vector fields](../../../../../../lie-bracket-of-vector-fields.md), whose action on a function is $X(Yf)-Y(Xf)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
