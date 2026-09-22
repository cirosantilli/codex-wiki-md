<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $R=\mathcal O_{X,x}$, $\mathfrak m=\mathfrak m_x$ and $d=\dim R$. Smoothness makes $R$ a [regular local ring](../../../../../../regular-local-ring.md), with [residue field](../../../../../../residue-field.md) $k$. A list of local parameters $t_1,\ldots,t_d$ is a [regular system of parameters](../../../../../../regular-system-of-parameters.md): its images form a basis of the [cotangent space of a local ring](../../../../../../cotangent-space-of-a-local-ring.md) $\mathfrak m/\mathfrak m^2$. Set $J=(t_1,\ldots,t_d)$. The basis condition says $\mathfrak m=J+\mathfrak m^2$, so the finitely generated module $\mathfrak m/J$ equals $\mathfrak m(\mathfrak m/J)$. The [Nakayama lemma](../../../../../../nakayama-lemma.md) gives

$$
\boxed{\mathfrak m=(t_1,\ldots,t_d).}
$$

We now construct the requested [formal power series](../../../../../../formal-power-series.md), rather than assert that a local function has a convergent expansion. The [associated graded ring of a regular local ring](../../../../../../associated-graded-ring-of-a-regular-local-ring.md) is

$$
\operatorname{gr}_{\mathfrak m}R\cong k[T_1,\ldots,T_d],\qquad T_i\longmapsto t_i\bmod\mathfrak m^2.
$$

Indeed these initial forms generate the graded ring, since the $t_i$ generate $\mathfrak m$. The [Dimension theorem for Noetherian local rings](../../../../../../dimension-theorem-for-noetherian-local-rings.md) gives $\dim\operatorname{gr}_{\mathfrak m}R=d$. A nonzero kernel in the surjection from the [polynomial ring](../../../../../../polynomial-ring.md) would make its quotient have dimension at most $d-1$, so that kernel is zero.

For $f\in R$, choose $P_0\in k$ to be its residue at $x$. Inductively suppose homogeneous polynomials $P_0,\ldots,P_{n-1}$ have been chosen such that

$$
r_n=f-\sum_{j<n}P_j(t_1,\ldots,t_d)\in\mathfrak m^n.
$$

The graded-ring isomorphism gives a unique homogeneous polynomial $P_n(T_1,\ldots,T_d)$ of degree $n$ representing the class of $r_n$ in $\mathfrak m^n/\mathfrak m^{n+1}$. Subtracting $P_n(t)$ makes the next remainder lie in $\mathfrak m^{n+1}$. Hence

$$
\boxed{f\longleftrightarrow\sum_{n\ge0}P_n(T_1,\ldots,T_d)\in k[[T_1,\ldots,T_d]].}
$$

This equality is interpreted in the [adic completion of a module](../../../../../../adic-completion-of-a-module.md) $\widehat R=\varprojlim R/\mathfrak m^n$. The same induction applies to every compatible sequence of residues in this inverse limit, so evaluation $T_i\mapsto t_i$ defines an isomorphism $k[[T_1,\ldots,T_d]]\cong\widehat R$. It is injective because the lowest nonzero homogeneous term of a series has nonzero initial form. The [Krull intersection theorem](../../../../../../krull-intersection-theorem.md) gives $\bigcap_n\mathfrak m^n=0$, so $R$ embeds in its completion and the series determines $f$. This is the [formal expansion at a smooth point](../../../../../../formal-expansion-at-a-smooth-point.md); it depends on the chosen [regular system of parameters](../../../../../../regular-system-of-parameters.md), and does not claim that the infinite sum converges inside $R$. If $d=0$, the [local ring](../../../../../../local-ring.md) is just $k$, and only the constant term is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
