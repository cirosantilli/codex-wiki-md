<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First we need all equality cases, rather than just the examples from part (c). The threshold estimate in part (b), with $t>0$, shows that any maximum-weight [k-Sperner family](../../../../../../k-sperner-family.md) has [Lubell mass](../../../../../../lubell-mass.md) exactly $k$.

For each $A\in\mathcal A$, let $\ell(A)$ be the largest number of members in a strict [chain in a partially ordered set](../../../../../../chain-in-a-partially-ordered-set.md) within $\mathcal A$ ending at $A$. Its values lie in $\{1,\ldots,k\}$. If $A\subsetneq B$ then $\ell(B)\geq\ell(A)+1$, so each height class $\mathcal A_j=\{A:\ell(A)=j\}$ is an [antichain](../../../../../../antichain.md). Its [Lubell mass](../../../../../../lubell-mass.md) is at most one by the [LYM inequality](../../../../../../lubell-yamamoto-meshalkin-inequality.md), and

$$
k=L(\mathcal A)=\sum_{j=1}^kL(\mathcal A_j).
$$

Consequently every height class has [Lubell mass](../../../../../../lubell-mass.md) one. By [equality in the LYM inequality](../../../../../../equality-in-the-lym-inequality.md), each is a full rank level. Since the classes are disjoint, the maximizing family is a union of exactly $k$ distinct full levels.

Let $t$ again be the $k$th largest $u(i)$, let $h$ ranks have $u(i)>t$, and let $s$ ranks have $u(i)=t$. Equality in the threshold estimate requires all $h$ higher-weight levels, no lower-weight levels, and any $k-h$ of the $s$ tied levels. Thus the [number of maximizing weighted k-Sperner families](../../../../../../number-of-maximizing-weighted-k-sperner-families.md) is

$$
m=\binom{s}{k-h},\qquad 0\leq h<k,\quad k-h\leq s\leq n+1-h.
$$

Conversely, every such $h,s$ is realizable. Assign $u(i)=2$ on $h$ chosen ranks, $u(i)=1$ on $s$ further ranks, and $u(i)=1/2$ on all remaining ranks, then set $w(i)=u(i)/\binom ni$. These weights are positive and have exactly the stated tie pattern.

Putting $j=k-h$ gives a concise classification of the possible integers:

$$
\boxed{\left\{\binom{s}{j}:1\leq j\leq k,\quad j\leq s\leq n+1-k+j\right\}.}
$$

Repeated values in this set are counted only once. The possible counts need not form an interval: for example, when $n=5,k=2$ they are $1,2,3,4,5,6,10,15$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
