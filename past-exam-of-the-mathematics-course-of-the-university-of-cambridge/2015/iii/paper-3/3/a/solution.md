<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $A=kQ$, $X_i=e_iX$, and let $f_\rho$ be the action of the arrow $\rho$ on $X_{s(\rho)}$. Write $P_i=Ae_i$, a left [projective module](../../../../../../projective-module.md). The [standard projective resolution of a quiver representation](../../../../../../standard-projective-resolution-of-a-quiver-representation.md) is

$$
\boxed{0\longrightarrow\bigoplus_{\rho\in Q_1}P_{t(\rho)}\otimes_kX_{s(\rho)}\xrightarrow{d}\bigoplus_{i\in Q_0}P_i\otimes_kX_i\xrightarrow{\varepsilon}X\longrightarrow0.}
$$

The algebra acts on the first tensor factor. The augmentation is $\varepsilon(p\otimes x)=px$. On the summand for $\rho:i\to j$, the differential sends $p\otimes x$ to $p\rho\otimes x$ in the $i$-summand minus $p\otimes f_\rho(x)$ in the $j$-summand. Here $p\in Ae_j$, so $p\rho\in Ae_i$. These formulas specify every term and map, and $\varepsilon d=0$.

Exactness is the standard path resolution fact: the relations identify a path acting on a vector with successively applying its arrows; uniqueness of the first traversed arrow supplies injectivity of the relation map. Each $Ae_i$ is a direct summand of $A$ because $e_i$ is an [idempotent](../../../../../../idempotent.md), and tensoring with a $k$-vector space gives a direct sum of copies of $Ae_i$. Both terms preceding $X$ are consequently [projective modules](../../../../../../projective-module.md). Thus the displayed sequence is a [projective resolution](../../../../../../projective-resolution.md) of length at most one.

The same path resolution works for arbitrary left modules, with possibly infinite-dimensional $X_i$ and arbitrary direct sums of [projective modules](../../../../../../projective-module.md). Hence every left $A$-module has projective dimension at most one. Equivalently, **$A$ is a left hereditary ring**: if $N\subseteq P$ with $P$ projective, dimension shifting gives $\operatorname{Ext}^1_A(N,M)\cong\operatorname{Ext}^2_A(P/N,M)=0$ for every $M$, so $N$ is projective. This argument also covers [quivers](../../../../../../quiver.md) with oriented cycles.

For dimension vectors $\mathbf n,\mathbf m\in\mathbb R^{Q_0}$, define the [Ringel form](../../../../../../ringel-form.md)

$$
\boxed{\langle\mathbf n,\mathbf m\rangle_Q=\sum_{i\in Q_0}n_im_i-\sum_{\rho\in Q_1}n_{s(\rho)}m_{t(\rho)}.}
$$

Apply $\operatorname{Hom}_A(-,Y)$ to the [projective resolution](../../../../../../projective-resolution.md). Evaluation at $e_i$ identifies $\operatorname{Hom}_A(P_i\otimes_kV,Y)$ with $\operatorname{Hom}_k(V,Y_i)$. Consequently there is an exact sequence

$$
0\longrightarrow\operatorname{Hom}_Q(X,Y)\longrightarrow C^0\xrightarrow{\delta}C^1\longrightarrow\operatorname{Ext}^1_Q(X,Y)\longrightarrow0,
$$

where

$$
C^0=\bigoplus_i\operatorname{Hom}_k(X_i,Y_i),\quad C^1=\bigoplus_\rho\operatorname{Hom}_k(X_{s(\rho)},Y_{t(\rho)}),\quad(\delta h)_\rho=g_\rho h_{s(\rho)}-h_{t(\rho)}f_\rho.
$$

This is the [extension complex of quiver representations](../../../../../../extension-complex-of-quiver-representations.md). Taking its alternating dimension sum yields

$$
\boxed{\dim\operatorname{Hom}_Q(X,Y)-\dim\operatorname{Ext}^1_Q(X,Y)=\langle\dim X,\dim Y\rangle_Q.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
