<h1 id="17g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $r=\operatorname{tr}C$, $s=\operatorname{tr}D$, and $\beta=(1-i)/2$. Their [traces](../../../../../../matrix-trace.md) are real by part c, and $\Phi(C)=\beta rI+iC$. Thus $\operatorname{tr}\Phi(C)=(2\beta+i)r=r$. Expanding the product and using $2\beta^2+2i\beta=1$ gives

$$
\operatorname{tr}(\Phi(C)\Phi(D))=rs-\operatorname{tr}(CD).
$$

Therefore

$$
\boxed{b(\Phi(C),\Phi(D))
=\frac12[rs-\operatorname{tr}(CD)-rs]
=-\frac12\operatorname{tr}(CD)=c(C,D).}
$$

In particular the [trace](../../../../../../matrix-trace.md) expression is real and symmetric on $Q$. Under the coordinates $C=aI+i\mathbf v\cdot\mathbf A$, $D=dI+i\mathbf w\cdot\mathbf A$, it is $-ad+\mathbf v\cdot\mathbf w$. Thus the [trace form on scalar-plus-skew-Hermitian two-by-two matrices](../../../../../../trace-form-on-scalar-plus-skew-hermitian-two-by-two-matrices.md) has **[rank](../../../../../../rank-one-quadratic-form.md) $4$, inertia $(3,1)$**, or numerical signature $2$, agreeing with $b$ under the real isomorphism.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
