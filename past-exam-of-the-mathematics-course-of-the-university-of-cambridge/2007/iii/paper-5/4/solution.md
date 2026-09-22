<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The objective is a continuous [faithful representation](../../../../../faithful-representation.md) of a [uniform pro-p group](../../../../../uniform-pro-p-group.md) $G$ in some $\operatorname{GL}_N(\mathbb Z_p)$. The proof proceeds from the intrinsic Lie lattice to a small [matrix group](../../../../../matrix-group.md), then extends the resulting representation to all of $G$. This last step matters: a representation defined only on an [open subgroup](../../../../../open-subgroup.md) does not yet establish linearity of the original [group](../../../../../group-split.md).

Let $L=L_G$ be the [Lie algebra of a uniform pro-p group](../../../../../lie-algebra-of-a-uniform-pro-p-group.md) and put $\mathfrak g=\mathbb Q_p\otimes_{\mathbb Z_p}L$. The uniform-group/Lie-lattice correspondence identifies the [group](../../../../../group-split.md) law on $L$ with BCH. The substantial finite-dimensional Lie-theoretic input is the [Ado theorem](../../../../../ado-s-theorem.md): every finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) over a characteristic-zero [field](../../../../../field.md) admits a faithful finite-dimensional representation. Apply it to obtain

$$
\rho:\mathfrak g\hookrightarrow\operatorname{End}_{\mathbb Q_p}(V),\qquad\rho([x,y])=\rho(x)\rho(y)-\rho(y)\rho(x).
$$

An [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) would not suffice here, since it kills the centre; Ado supplies [injectivity](../../../../../injective-function.md) even in central directions.

Choose a [p-adic lattice](../../../../../integral-lattice-in-a-p-adic-vector-space.md) $\Lambda$ spanning $V$. Since $L$ has finitely many lattice generators, their representing [matrices](../../../../../matrix.md) have bounded denominators. There is therefore an integer $a\ge0$ such that

$$
\rho(p^aL)\subseteq p^\epsilon\operatorname{End}_{\mathbb Z_p}(\Lambda),\qquad\epsilon=\begin{cases}1,&p\ne2,\\2,&p=2.\end{cases}
$$

On this [matrix](../../../../../matrix.md) lattice the series $\exp X=\sum_{n\ge0}X^n/n!$ and $\log(1+Y)=\sum_{n\ge1}(-1)^{n+1}Y^n/n$ converge and are inverse. For example $v_p(n!)\le n/(p-1)$, so the valuations of the exponential terms tend to infinity with this choice of $\epsilon$; the [logarithm](../../../../../logarithm.md) terms do as well. They take values in $1+p^\epsilon\operatorname{End}(\Lambda)$ and in $p^\epsilon\operatorname{End}(\Lambda)$ respectively. The formal identity $\exp(\operatorname{BCH}(X,Y))=\exp X\exp Y$ holds for the convergent series.

Under the correspondence, $U=G^{p^a}$ has Lie lattice $p^aL$ and is an open [characteristic subgroup](../../../../../characteristic-subgroup.md). Define

$$
\eta:U\longrightarrow\operatorname{GL}(\Lambda),\qquad\eta(u)=\exp(\rho(\log_Gu)),
$$

where $\log_G$ denotes the identification of $U$ with $p^aL$. A Lie [homomorphism](../../../../../homomorphism.md) preserves BCH, so the exponential identity proves $\eta(uv)=\eta(u)\eta(v)$. If $\eta(u)=I$, the [matrix](../../../../../matrix.md) [logarithm](../../../../../logarithm.md) gives $\rho(\log_Gu)=0$; faithfulness of $\rho$ gives $u=1$. Thus $\eta$ is a continuous faithful integral representation of $U$.

To extend it, take the [module](../../../../../module-mathematics.md)

$$
W=\{f:G\to\Lambda:f(ux)=\eta(u)f(x)\text{ for all }u\in U,\ x\in G\}.
$$

Values on a transversal of $U\backslash G$ determine $f$, so $W$ is a [free module](../../../../../free-module.md) over $\mathbb Z_p$ of rank $[G:U]\dim V$. These functions are continuous, since on each open [coset](../../../../../coset.md) they are given by the continuous representation $\eta$. Define $(T_gf)(x)=f(xg)$. The equivariance condition is preserved, and $T_gT_h=T_{gh}$. In a transversal [basis](../../../../../basis.md) each $T_g$ is a permutation of blocks followed by [matrices](../../../../../matrix.md) from $\eta(U)$, so it belongs to $\operatorname{GL}(W)$ and depends continuously on $g$.

Faithfulness can be checked directly. If $g\notin U$, right multiplication moves the [coset](../../../../../coset.md) $U$ to a different [coset](../../../../../coset.md), so $T_g$ moves a function supported on one block and cannot be the identity. If $g\in U$ and $T_g=1$, evaluation at $1$ gives $f(g)=f(1)$ for every $f$, whereas equivariance gives $f(g)=\eta(g)f(1)$. Since $f(1)$ is arbitrary, $\eta(g)=I$, and hence $g=1$. Therefore

$$
\boxed{G\hookrightarrow\operatorname{GL}_{[G:U]\dim V}(\mathbb Z_p).}
$$

[Compactness](../../../../../compact-space.md) of $G$ makes this continuous injection a [homeomorphism](../../../../../homeomorphism.md) onto its closed image. This proves the [linearity of a uniform pro-p group](../../../../../linearity-of-a-uniform-pro-p-group.md) for the full [group](../../../../../group-split.md), including its centre, and explains why taking a sufficiently small power lattice permits [matrix](../../../../../matrix.md) integration before finite-index induction restores the whole [group](../../../../../group-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
