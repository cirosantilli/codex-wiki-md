<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For each [place of a number field](../../../../../place-of-a-number-field.md) $v$, let $K_v$ be the corresponding completion, and for finite $v$ let $\mathcal O_v$ be its [valuation ring](../../../../../valuation-ring.md). The [adele ring](../../../../../adele-ring.md) is the [restricted product](../../../../../restricted-product.md)

$$
\mathbb A_K=\prod_v'K_v
=\left\{(x_v)_v:x_v\in\mathcal O_v\text{ for all but finitely many finite }v\right\}.
$$

Its [restricted product topology](../../../../../restricted-product-topology.md) has basic open sets $\prod_vU_v$, where every $U_v\subseteq K_v$ is open and $U_v=\mathcal O_v$ at all but finitely many finite places.

First take $K=\mathbb Q$. The neighborhood

$$
(-1/2,1/2)\times\prod_p\mathbb Z_p
$$

of zero meets the diagonal copy of $\mathbb Q$ only in zero: a rational number lying in every $\mathbb Z_p$ is an [integer](../../../../../integer.md), and the only integer in the indicated real interval is zero. Thus $\mathbb Q$ is discrete in $\mathbb A_{\mathbb Q}$.

Every rational adele is congruent modulo $\mathbb Q$ to an element of

$$
[0,1]\times\prod_p\mathbb Z_p.
$$

Indeed, the finitely many negative $p$-adic principal parts can be removed simultaneously by subtracting a rational number, using the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md); subtracting an integer then moves the real component into $[0,1]$. This set is compact by the compactness of $[0,1]$, the compactness of every $\mathbb Z_p$, and the [Tychonoff theorem](../../../../../tychonoff-s-theorem.md). Its image covers the quotient, so $\mathbb A_{\mathbb Q}/\mathbb Q$ is compact.

Now choose a $\mathbb Q$-basis of the [number field](../../../../../number-field.md) $K$. The given topological isomorphism

$$
\mathbb A_{\mathbb Q}\otimes_{\mathbb Q}K\simeq\mathbb A_K
$$

identifies the additive pair $(\mathbb A_K,K)$ with $(\mathbb A_{\mathbb Q}^n,\mathbb Q^n)$. A finite product of discrete subgroups is discrete, and

$$
\mathbb A_K/K\simeq(\mathbb A_{\mathbb Q}/\mathbb Q)^n
$$

is compact.

The [idele group](../../../../../idele-group.md) is

$$
J_K=\prod_v'K_v^\times,
$$

where the distinguished subgroup at a finite place is $\mathcal O_v^\times$. It carries the corresponding [restricted product topology on the idele group](../../../../../restricted-product-topology-on-the-idele-group.md). The inclusion $j:J_K\to\mathbb A_K$ is continuous: the inverse image of a basic adelic open set is locally a product of open subsets of $K_v^\times$, and outside finitely many places every idele component already belongs to $\mathcal O_v^\times\subseteq\mathcal O_v$.

It is not a homeomorphism onto its image. Let $p_i$ be the $i$th rational prime and define the idele $x^{(i)}$ to equal $p_i$ at the place over $p_i$ and $1$ everywhere else. In the adele topology, $x^{(i)}\to1$: the difference is zero at every fixed place once $i$ is large, while $p_i-1\in\mathbb Z_{p_i}$ at the single moving place. In the idele topology the sequence does not converge to $1$, because the open neighborhood

$$
\prod_{v\mid\infty}K_v^\times\times\prod_{v\nmid\infty}\mathcal O_v^\times
$$

contains no $x^{(i)}$: its $p_i$-component has positive valuation and is not a unit. Hence the inverse of $j$ on its image is not continuous.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 123](../../paper-123-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
