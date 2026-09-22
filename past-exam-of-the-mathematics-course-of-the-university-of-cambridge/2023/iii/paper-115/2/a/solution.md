<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In local coordinates, for

$$
\alpha=\frac1{r!}\alpha_{i_1\ldots i_r}\,
dx^{i_1}\wedge\cdots\wedge dx^{i_r},
$$

the [exterior derivative](../../../../../../exterior-derivative.md) is

$$
d\alpha=\frac1{r!}\frac{\partial\alpha_{i_1\ldots i_r}}{\partial x^j}
dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.
$$

Applying $d$ again gives symmetric second partial derivatives contracted with the antisymmetric wedge $dx^k\wedge dx^j$, hence $d^2=0$. Expanding coefficients and moving $d\alpha$ past a degree-$r$ form gives the graded Leibniz rule

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta.
$$

For a function $f$ and smooth $F:X\to Y$, the chain rule gives

$$
d(F^*f)=d(f\circ F)=F^*(df).
$$

Every differential form is locally a sum of products $f_0\,df_1\wedge\cdots\wedge df_r$. Since pullback preserves products and wedge products, the function case and the graded Leibniz rule imply

$$
d(F^*\alpha)=F^*(d\alpha)
$$

for every form.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
