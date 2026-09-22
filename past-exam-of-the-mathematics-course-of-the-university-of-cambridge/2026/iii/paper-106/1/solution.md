<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Schauder basis](../../../../../schauder-basis.md) of a real [Banach space](../../../../../banach-space-split.md) $X$ is a sequence $(e_n)$ for which every $x\in X$ has a unique norm-convergent expansion $x=\sum_na_ne_n$. Its [basis projection](../../../../../basis-projection.md) is

$$
P_nx=\sum_{k=1}^na_ke_k,
$$

and its [basis constant](../../../../../basis-constant.md) is $K_b=\sup_n\lVert P_n\rVert<\infty$.

For the sequence space $Y$ in the question, define

$$
J:Y\longrightarrow X,
\qquad
J(a)=\sum_{n=1}^\infty a_ne_n.
$$

Convergence in the definition of $Y$ makes $J$ well defined, and uniqueness of basis coefficients makes it a [linear bijection](../../../../../linear-isomorphism.md). Moreover,

$$
\lVert J(a)\rVert
=\lim_n\left\lVert\sum_{k=1}^na_ke_k\right\rVert
\leq\lVert a\rVert_Y,
$$

whereas

$$
\lVert a\rVert_Y
=\sup_n\lVert P_nJ(a)\rVert
\leq K_b\lVert J(a)\rVert.
$$

Thus $J$ is an [isomorphism](../../../../../isomorphism-of-banach-spaces.md) and, in particular, the displayed supremum really is a complete norm on $Y$.

The [coordinate functional of a Schauder basis](../../../../../coordinate-functional-of-a-schauder-basis.md) is

$$
e_n^*\left(\sum_ka_ke_k\right)=a_n.
$$

It is bounded because $a_ne_n=(P_n-P_{n-1})x$. On finite linear combinations of the $e_n^*$, the nth partial-sum operator is the restriction of $P_n^*$, since

$$
P_n^*e_j^*=\begin{cases}e_j^*,&j\leq n,\\0,&j>n.\end{cases}
$$

The operators have norms at most $K_b$, so the standard basis criterion shows that the [dual sequence of a Schauder basis](../../../../../dual-sequence-of-a-schauder-basis.md) $(e_n^*)$ is a [basic sequence](../../../../../basic-sequence.md) in $X^*$. For every $x^*\in X^*$ and $x\in X$,

$$
\langle P_n^*x^*,x\rangle
=\langle x^*,P_nx\rangle
\longrightarrow\langle x^*,x\rangle,
$$

which is precisely $P_n^*x^*\to x^*$ in the [weak-star topology](../../../../../weak-star-topology.md).

Suppose now that $X$ is a [reflexive Banach space](../../../../../reflexive-banach-space.md). If $\lVert x^*-P_n^*x^*\rVert$ did not tend to zero, approximation by finite basis blocks would give a bounded block sequence $(u_j)$ and an $\varepsilon>0$ such that $|x^*(u_j)|\geq\varepsilon$. Reflexivity gives a weakly convergent subsequence. Every fixed coordinate functional is eventually zero on a block sequence, so its weak limit has every basis coordinate zero and is therefore zero. This contradicts $|x^*(u_j)|\geq\varepsilon$. Hence $P_n^*x^*\to x^*$ in norm for every $x^*$, so the basis is [shrinking](../../../../../shrinking-schauder-basis.md) and $(e_n^*)$ is a basis of $X^*$.

The converse fails. The standard basis of $c_0$ is shrinking because its dual sequence is the standard basis of $\ell^1=(c_0)^*$, but $c_0$ is not [reflexive](../../../../../reflexive-banach-space.md).

Finally assume $(e_n^*)$ is a basis of $X^*$. Map $x^{**}\in X^{**}$ to

$$
a_n=x^{**}(e_n^*).
$$

For $s_n=\sum_{k=1}^na_ke_k$,

$$
\lVert s_n\rVert
=\sup_{\lVert x^*\rVert\leq1}
|x^{**}(P_n^*x^*)|
\leq K_b\lVert x^{**}\rVert,
$$

so $(a_n)\in Z$. Conversely, if $(a_n)\in Z$ and $M=\sup_n\lVert s_n\rVert$, define

$$
F(x^*)=\lim_nx^*(s_n).
$$

The limit exists: for $m>n$,

$$
|x^*(s_m-s_n)|
\leq2M\lVert x^*-P_n^*x^*\rVert\longrightarrow0
$$

because $(e_n^*)$ is a basis. Also $|F(x^*)|\leq M\lVert x^*\rVert$, so $F\in X^{**}$ and $F(e_n^*)=a_n$. These two constructions are inverse and satisfy

$$
\lVert F\rVert\leq\lVert(a_n)\rVert_Z
\leq K_b\lVert F\rVert.
$$

Thus $X^{**}$ and $Z$ are isomorphic.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
