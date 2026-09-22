<h1 id="5d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Cauchy's theorem for finite groups](../../../../../../cauchy-theorem-for-groups.md) states that if a [prime number](../../../../../../prime-number.md) $p$ divides the order of a finite group $G$, then $G$ contains an element of order $p$.

Consider

$$
X=\{(x_1,\ldots,x_p)\in G^p:x_1x_2\cdots x_p=e\}.
$$

The first $p-1$ entries determine the last, so $|X|=|G|^{p-1}$ is divisible by $p$. The [cyclic group](../../../../../../cyclic-group.md) $C_p$ acts on $X$ by cyclically shifting the coordinates; the shifted tuple remains in $X$ because $x_2\cdots x_px_1=x_1^{-1}(x_1\cdots x_p)x_1=e$. Every [orbit](../../../../../../orbit-dynamical-system.md) has size one or $p$. The fixed points are exactly $(x,\ldots,x)$ with $x^p=e$. Their number is therefore divisible by $p$. Since the identity is one fixed point, another exists; its order is $p$.

Now let the [abelian group](../../../../../../abelian-group.md) $G$ have order $pq$ for distinct primes $p,q$. Cauchy's theorem supplies $x,y$ of orders $p,q$. Their cyclic subgroups intersect trivially, and commutativity shows that $xy$ has order $pq$. Thus $G$ is cyclic and

$$
\boxed{G\cong C_{pq}\cong C_p\times C_q}.
$$

The corresponding assertion for order $p^2$ is false: $C_{p^2}$ is not isomorphic to $C_p\times C_p$, since the former has an element of order $p^2$ while every nonidentity element of the latter has order $p$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
