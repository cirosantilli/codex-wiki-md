<h1 id="6d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We first prove the needed instance of [Cauchy theorem for groups](../../../../../../cauchy-theorem-for-groups.md), rather than invoke it. Let a [prime number](../../../../../../prime-number.md) $q$ divide $|G|$ and consider the set

$$
\mathcal T=\{(g_1,\ldots,g_q):g_1\cdots g_q=1\}.
$$

There are $|G|^{q-1}$ such tuples: choose the first $q-1$ entries freely, and the last is forced. Cyclic rotation preserves this set, because moving the first entry to the end conjugates the product, which remains $1$. Each rotation [orbit of a group action](../../../../../../orbit-of-a-group-action.md) has either one or $q$ elements. Indeed a nontrivial shift fixing a tuple generates all shifts, since its step has an inverse modulo the prime $q$. The fixed tuples are precisely $(g,\ldots,g)$ with $g^q=1$.

Counting nonfixed orbits in multiples of $q$, and using $q\mid |G|^{q-1}$, shows that the number of solutions of $g^q=1$ is divisible by $q$. The identity supplies one solution, so there is a nonidentity solution. If its [order of a group element](../../../../../../order-of-a-group-element.md) is $d$, divide $q$ by $d$: the remainder would give a smaller positive exponent producing the identity, so $d\mid q$. Hence $d=q$. This proves the required prime-order existence result by the [cyclic-tuple proof of Cauchy theorem](../../../../../../cyclic-tuple-proof-of-cauchy-theorem.md).

Our hypothesis says that this nonidentity element has order $p$, so $q=p$. Every prime divisor of $|G|$ is therefore $p$, which gives

$$
\boxed{|G|=p^n\quad\text{for some }n\ge0.}
$$

Thus a [finite group of prime exponent has prime-power order](../../../../../../finite-group-of-prime-exponent-has-prime-power-order.md). The case $n=0$ includes the trivial [group](../../../../../../group-split.md). No [group](../../../../../../group-split.md)-theoretic counting theorem was assumed in the tuple argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
