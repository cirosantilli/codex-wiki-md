<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

An element of the [general linear group over a finite field](../../../../../general-linear-group-over-a-finite-field.md) is an invertible $2\times2$ [matrix](../../../../../matrix.md). Its columns must form an ordered [basis](../../../../../basis.md) of $\mathbb F_p^2$. There are $p^2-1$ choices for the first column. Its [linear span](../../../../../linear-span.md) contains $p$ vectors, so there are $p^2-p$ choices for a second column outside that [linear span](../../../../../linear-span.md). Thus the [order of a general linear group over a finite field](../../../../../order-of-a-general-linear-group-over-a-finite-field.md) is

$$
\boxed{|GL_2(\mathbb F_p)|=(p^2-1)(p^2-p)=p(p-1)^2(p+1).}
$$

The [determinant](../../../../../determinant.md) is a surjective [group homomorphism](../../../../../group-homomorphism.md) $GL_2(\mathbb F_p)\to\mathbb F_p^\times$: for each $a\ne0$, the diagonal [matrix](../../../../../matrix.md) $\operatorname{diag}(a,1)$ has [determinant](../../../../../determinant.md) $a$. Its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is the [special linear group over a finite field](../../../../../special-linear-group-over-a-finite-field.md). The [first isomorphism theorem](../../../../../first-isomorphism-theorem.md) gives $|GL_2|/|SL_2|=p-1$, hence

$$
\boxed{|SL_2(\mathbb F_p)|=p(p^2-1).}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
