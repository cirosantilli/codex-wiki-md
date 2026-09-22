<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Z_t$ denote the generation-$t$ type-count [vector](../../../../../../vector.md), and let $p_i^{(t)}=\Pr_i(|Z_t|>0)$ from a single type-$i$ ancestor. Every type-$j$ child independently has [probability](../../../../../../probability.md) $p_j^{(t)}$ of having descendants in generation $t$. For a [Poisson random variable](../../../../../../poisson-distribution.md) $N$ with [mean](../../../../../../expected-value.md) $\lambda$, $\mathbb E s^N=\exp[\lambda(s-1)]$. Independence across child types therefore gives

$$
p^{(0)}=\mathbf1,\qquad p_i^{(t+1)}=1-\prod_j\exp(-\lambda_{ij}p_j^{(t)})=T_i(p^{(t)}),\qquad T_i(x)=1-e^{-(\Lambda x)_i}.
$$

The events of nonempty successive generations decrease. Each individual has finitely many children almost surely, so the total tree is infinite precisely when no generation is empty. Consequently $p^{(t)}\downarrow p$, the actual [survival probability of a branching process](../../../../../../survival-probability-of-a-branching-process.md). Continuity of $T$ yields

$$
\boxed{p_i=1-\exp\left(-\sum_j\lambda_{ij}p_j\right).}
$$

The map $T$ is coordinatewise increasing on nonnegative [vectors](../../../../../../vector.md). Every nonnegative [fixed point](../../../../../../fixed-point.md) $p'$ automatically lies in $[0,1]^l$, since its coordinates equal $1-e^{-z}$ with finite $z\ge0$. Hence $p'\le\mathbf1$ and, by induction, $p'=T^t(p')\le T^t(\mathbf1)=p^{(t)}$. Taking limits proves **$p'\le p$ in every coordinate**, so $p$ is the greatest nonnegative solution, not merely some [fixed point](../../../../../../fixed-point.md). This argument applies without irreducibility assumptions to the [multitype Poisson branching process](../../../../../../multitype-poisson-branching-process.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
