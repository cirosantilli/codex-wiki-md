<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A=(a_{ij})$, $b=(b_i)$, $\mathbf1=(1,1,1)^T$, and $c=A\mathbf1$. From the displayed tableau,

$$
c=\left(0,\frac35-\frac{\sqrt6}{10},
\frac35+\frac{\sqrt6}{10}\right)^T.
$$

The quadrature moments satisfy

$$
b^Tc^q=\frac1{q+1},\qquad q=0,1,2,3,4.
$$

Direct substitution into the remaining [Butcher order conditions](../../../../../../butcher-order-condition.md) gives, for example,

$$
b^TAc=\frac16,\quad
b^T(c\circ Ac)=\frac18,\quad
b^TA(c\circ c)=\frac1{12},\quad
b^TA^2c=\frac1{24},
$$

and all rooted-tree conditions of orders at most five are satisfied. The order-six moment already fails:

$$
b^Tc^5=\frac{33}{200}\ne\frac16.
$$

The [Runge-Kutta method](../../../../../../runge-kutta-method.md) therefore has

$$
\boxed{\text{order }5}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
