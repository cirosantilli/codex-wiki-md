<h1 id="20g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Evaluation at $\alpha$ gives the ring isomorphism

$$
\mathcal O_L\cong\mathbb Z[X]/(f),
$$

and reducing modulo $p$ gives

$$
\mathcal O_L/p\mathcal O_L
\cong\mathbb F_p[X]/(\overline f).
$$

For each $i$,

$$
\mathcal O_L/P_i
\cong\mathbb F_p[X]/(\overline g_i).
$$

This quotient is a field because $\overline g_i$ is irreducible. Hence $P_i$ is a nonzero [prime ideal](../../../../../../prime-ideal.md); it is nonzero because it contains $p$. Its [ideal norm](../../../../../../ideal-norm.md) is

$$
\boxed{N(P_i)=|\mathcal O_L/P_i|
=p^{\deg\overline g_i}.}
$$

The ideals are distinct. Indeed, if $P_i=P_j$ with $i\ne j$, then both $\overline g_i$ and $\overline g_j$ would vanish in the same quotient. Since distinct monic irreducibles are coprime, a [Bezout identity](../../../../../../bezout-identity.md) between them would make $1$ vanish there, a contradiction.

Because the chosen lifts satisfy

$$
f(X)=\prod_{i=1}^r g_i(X)^{e_i}+pH(X)
$$

for some $H\in\mathbb Z[X]$, evaluation at $\alpha$ gives

$$
\prod_i g_i(\alpha)^{e_i}\in p\mathcal O_L.
$$

Every generator of the product ideal $\prod_iP_i^{e_i}$ either contains a factor $p$ or is the displayed product, so

$$
\prod_iP_i^{e_i}\subseteq p\mathcal O_L.
$$

On the other hand, multiplicativity of ideal norms and $\sum_i e_i\deg\overline g_i=\deg f=[L:\mathbb Q]$ give

$$
N\!\left(\prod_iP_i^{e_i}\right)
=p^{\sum_i e_i\deg\overline g_i}
=p^{[L:\mathbb Q]}
=N(p\mathcal O_L).
$$

Two finite-index ideals with one contained in the other and equal index are equal. Thus the [Dedekind factorization theorem](../../../../../../dedekind-factorization-theorem.md) is proved in this monogenic case:

$$
\boxed{p\mathcal O_L=P_1^{e_1}\cdots P_r^{e_r}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20G](../../20g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
