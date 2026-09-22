<h1 id="8g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose that $Q$ were not surjective. Its image would be a proper subspace of $F^n$, so there would be a nonzero functional

$$
\ell(y_1,\ldots,y_n)=\sum_{j=1}^nc_jy_j
$$

vanishing on $\operatorname{im}Q$. Then

$$
0=\ell(Qx)=\sum_{j=1}^nc_jq_j(x)
$$

for every $x\in V$, contradicting the linear independence of the $q_j$. Hence the [surjectivity of independent linear functionals](../../../../../../surjectivity-of-independent-linear-functionals.md) gives

$$
\boxed{Q:V\to F^n\text{ is surjective}}.
$$

Let $K=\bigcap_j\ker q_j=\ker Q$ and suppose $K\subseteq\ker f$. Define

$$
g:F^n\to F,
\qquad
g(Qx)=f(x).
$$

This is well-defined: if $Qx=Qy$, then $x-y\in K$, so $f(x)=f(y)$. It is linear, and surjectivity of $Q$ means it is defined on all of $F^n$. Thus there are [scalars](../../../../../../scalar.md) $a_1,\ldots,a_n$ such that $g(y)=\sum_ja_jy_j$. Therefore

$$
f(x)=g(Qx)=\sum_{j=1}^na_jq_j(x),
$$

and hence

$$
\boxed{f\in\operatorname{span}\{q_1,\ldots,q_n\}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8G](../../8g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
