<h1 id="7d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [Lagrange's theorem](../../../../../../lagrange-s-theorem.md), a [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) of $G$ has order $p^j$ for some $0\leq j\leq n$. The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) therefore gives

$$
|Y|=p^{n-j}.
$$

Thus an [orbit of a group action](../../../../../../orbit-of-a-group-action.md) either has one element or has size divisible by $p$, even if the acted-on set is infinite.

Apply this to the [conjugation action](../../../../../../conjugation-action.md). Its singleton [orbits of a group action](../../../../../../orbit-of-a-group-action.md) are the elements of the [centre of a group](../../../../../../center-of-a-group.md), while every other orbit has size divisible by $p$. Partitioning the finite [group](../../../../../../group-split.md) into these orbits gives the [class equation](../../../../../../class-equation.md), and hence

$$
|Z(G)|\equiv|G|\equiv0\pmod p.
$$

Since the identity belongs to $Z(G)$, its order is positive and divisible by $p$. Consequently

$$
\boxed{|Z(G)|\geq p>1.}
$$

Now suppose that $|Z(G)|=p^{n-1}$. It is then proper, so choose $x\notin Z(G)$. The [centralizer](../../../../../../centralizer.md)

$$
C_G(x)=\{g\in G:gx=xg\}
$$

is a [subgroup](../../../../../../subgroup.md): commuting with $x$ is preserved by multiplication and inverses. It contains $Z(G)$ and also $x$, so $|C_G(x)|>|Z(G)|=p^{n-1}$. By [Lagrange's theorem](../../../../../../lagrange-s-theorem.md), its order is a power of $p$ dividing $p^n$, forcing $C_G(x)=G$. But that would make $x$ central, a contradiction. Therefore

$$
\boxed{|Z(G)|\ne p^{n-1}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7D](../../7d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
