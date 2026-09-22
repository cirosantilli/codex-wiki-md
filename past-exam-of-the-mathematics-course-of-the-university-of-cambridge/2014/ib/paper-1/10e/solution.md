<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

If $|G|=p^a m$ with $p\nmid m$, a [Sylow subgroup](../../../../../sylow-subgroup.md) for $p$ is a subgroup of order $p^a$. The [Sylow theorems](../../../../../sylow-theorems.md) assert: such subgroups exist; every $p$-subgroup is contained in a Sylow subgroup; all Sylow $p$-subgroups are conjugate; and their number $n_p$ divides $m$ and satisfies $n_p\equiv1\pmod p$.

For [groups of order p squared q are not simple](../../../../../groups-of-order-p-squared-q-are-not-simple.md), if $p>q$, then $n_p\mid q$ and $n_p\equiv1\pmod p$ force $n_p=1$. Its unique Sylow subgroup is a nontrivial proper [normal subgroup](../../../../../normal-subgroup.md). Suppose instead $p<q$. If either Sylow count is one, the conclusion already follows. Otherwise $n_p=q$, while $n_q$ is either $p$ or $p^2$. The value $p$ is impossible because $0<p-1<q$. Thus $n_q=p^2$, and $q\mid(p^2-1)=(p-1)(p+1)$. Primality and $q>p$ imply $q\mid p+1$, hence $q=p+1$. The only consecutive primes are $p=2,q=3$.

In that exceptional order-$12$ case, four distinct Sylow $3$-subgroups contribute eight distinct nonidentity elements: their intersections are trivial. Only three nonidentity elements remain. Every subgroup of order four must contain exactly those remaining three, so there can be only one Sylow $2$-subgroup, contradicting the assumption that both counts were nontrivial. Therefore **no group of order $p^2q$ with distinct primes is simple**.

For the final factorization, normality of $H$ ensures $g^{-1}Pg$ is a Sylow $p$-subgroup of $H$. By Sylow conjugacy within $H$, choose $h\in H$ such that $g^{-1}Pg=h^{-1}Ph$. Then $k=gh^{-1}$ satisfies

$$
kPk^{-1}=gh^{-1}Phg^{-1}=P.
$$

Thus $k\in N_G(P)$ and $g=kh$. We have proved the [Frattini argument](../../../../../frattini-argument.md)

$$
\boxed{G=N_G(P)H.}
$$

The [normaliser](../../../../../normalizer.md) factorization includes the case $P=\{1\}$, when its normalizer is all of $G$.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
