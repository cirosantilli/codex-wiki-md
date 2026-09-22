<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expanding the symmetric spatial stencil by the [Taylor theorem](../../../../../../taylor-theorem.md) gives

$$
L_hu=\frac{\alpha+2\beta+2\gamma}{h^2}u+(\beta+4\gamma)u_{xx}+\frac{h^2}{12}(\beta+16\gamma)u_{xxxx}+\frac{h^4}{360}(\beta+64\gamma)u_{xxxxxx}+O(h^6).
$$

[Consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) and cancellation of the $h^2$ term require $\alpha+2\beta+2\gamma=0$, $\beta+4\gamma=1$, and $\beta+16\gamma=0$. Solving this [linear system](../../../../../../system-of-linear-equations.md) gives

$$
\boxed{\alpha=-\frac52,\qquad\beta=\frac43,\qquad\gamma=-\frac1{12}}.
$$

The resulting [fourth-order centered second derivative](../../../../../../fourth-order-centered-second-derivative.md) has

$$
L_hu=u_{xx}-\frac{h^4}{90}u_{xxxxxx}+O(h^6).
$$

The nonzero next coefficient proves that **the highest spatial [order of a numerical method](../../../../../../order-of-a-numerical-method.md) is four** for this three-parameter stencil.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
