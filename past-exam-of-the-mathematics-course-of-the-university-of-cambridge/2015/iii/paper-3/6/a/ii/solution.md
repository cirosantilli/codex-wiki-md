<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $X$ is indecomposable, part (i) makes it a [brick module](../../../../../../../brick-module.md). For its nonzero [dimension vector of a quiver representation](../../../../../../../dimension-vector-of-a-quiver-representation.md) $\mathbf n$,

$$
0<q_Q(\mathbf n)=1-\dim\operatorname{Ext}^1_Q(X,X)\leq1.
$$

The [Tits form of a quiver](../../../../../../../tits-form-of-a-quiver.md) takes integer values on integer vectors, so **$q_Q(\mathbf n)=1$ and $X$ has no self-extensions**.

Conversely, suppose $\mathbf n$ has nonnegative integer entries and $q_Q(\mathbf n)=1$. Choose a representation $M$ of that dimension vector whose orbit has maximal dimension. Such an orbit exists because dimensions are integers bounded by $\dim\operatorname{Rep}_Q(\mathbf n)$. If $M=U\oplus V$ with nonzero $U,V$, a nonzero extension in either direction would, by part 5(c), produce a middle representation of the same dimension vector with larger orbit. Hence $\operatorname{Ext}^1_Q(U,V)=\operatorname{Ext}^1_Q(V,U)=0$.

Writing $\mathbf u=\dim U$ and $\mathbf v=\dim V$, the [Ringel form](../../../../../../../ringel-form.md) identity then gives

$$
\begin{aligned}
1=q_Q(\mathbf u+\mathbf v)&=q_Q(\mathbf u)+q_Q(\mathbf v)+\langle\mathbf u,\mathbf v\rangle_Q+\langle\mathbf v,\mathbf u\rangle_Q\\
&=q_Q(\mathbf u)+q_Q(\mathbf v)+\dim\operatorname{Hom}_Q(U,V)+\dim\operatorname{Hom}_Q(V,U)\geq2.
\end{aligned}
$$

The last inequality uses positive integral values of $q_Q$ at both nonzero vectors. This contradiction makes $M$ indecomposable. Thus **the indecomposable dimension vectors are exactly the positive roots $q_Q(\mathbf n)=1$**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
