<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a basis $T_a$ of the [Lie algebra](../../../../../../lie-algebra-split.md), with $[T_b,T_c]=c^a{}_{bc}T_a$. On the [Matrix Lie group](../../../../../../matrix-lie-group.md) set

$$
\lambda=g^{-1}dg=T_a\lambda^a,\qquad \rho=dg\,g^{-1}=T_a\rho^a.
$$

Left multiplication by a constant matrix preserves $\lambda$, while right multiplication preserves $\rho$. Differentiating $g^{-1}g=I$ gives $d(g^{-1})=-g^{-1}(dg)g^{-1}$. Apply the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md) to obtain

$$
d\lambda=-\lambda\wedge\lambda,
\qquad d\rho=+\rho\wedge\rho.
$$

Because the [wedge product](../../../../../../exterior-product.md) antisymmetrizes the matrix products, these [Maurer-Cartan equations](../../../../../../maurer-cartan-equation.md) become

$$
\boxed{d\lambda^a=-\tfrac12c^a{}_{bc}\lambda^b\wedge\lambda^c,
\qquad d\rho^a=+\tfrac12c^a{}_{bc}\rho^b\wedge\rho^c.}
$$

Follow the vector-field naming used in the question: $L_a(g)=T_ag$ is right-invariant and generates left multiplication, whereas $R_a(g)=gT_a$ is left-invariant and generates right multiplication. They are dual to $\rho^a$ and $\lambda^a$, respectively. For any [one-form](../../../../../../one-form.md) $\eta$, $d\eta(X,Y)=X(\eta(Y))-Y(\eta(X))-\eta([X,Y])$. Evaluating the two [Maurer-Cartan equations](../../../../../../maurer-cartan-equation.md) on the corresponding invariant fields yields

$$
\boxed{[L_a,L_b]=-c^c{}_{ab}L_c,\qquad[R_a,R_b]=c^c{}_{ab}R_c,\qquad[L_a,R_b]=0.}
$$

For the last identity, the left and right multiplication flows commute. The opposite sign for the [right-invariant vector fields](../../../../../../right-invariant-vector-field.md) is therefore intrinsic; the letters attached to the two families are only a convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
