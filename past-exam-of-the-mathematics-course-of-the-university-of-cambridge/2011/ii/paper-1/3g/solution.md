<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Each nonidentity element of the [special orthogonal group](../../../../../special-orthogonal-group.md) $\operatorname{SO}(3)$ is a rotation fixing exactly the two unit vectors along its axis. Since $G$ is a [finite group](../../../../../finite-group.md), $\Omega$ is finite. If $v\in\Omega$ is fixed by $g\ne1$ and $h\in G$, then $hv$ is fixed by $hgh^{-1}\ne1$. Hence $G$ acts on $\Omega$ by a [group action](../../../../../group-action.md).

Let $N=|G|>1$, let $r$ be the number of [orbits of a group action](../../../../../orbit-of-a-group-action.md), and choose representatives with [stabilizer subgroups](../../../../../stabilizer-subgroup.md) of orders $n_1,\ldots,n_r$, each at least two. Count pairs $(g,v)$ with $g\ne1$ and $gv=v$. Counting by $g$ gives $2(N-1)$. Counting by [group orbits](../../../../../orbit-of-a-group-action.md) and using the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives

$$
\sum_{j=1}^r\frac N{n_j}(n_j-1)=2(N-1),\qquad
\sum_{j=1}^r\left(1-\frac1{n_j}\right)=2-\frac2N<2.
$$

Every summand is at least $1/2$, so $r<4$: **there are at most three orbits**. For the trivial [group](../../../../../group-split.md), $\Omega$ is empty and the assertion also holds.

For the rotation group of a regular [dodecahedron](../../../../../dodecahedron.md), $N=60$. The three [group orbits](../../../../../orbit-of-a-group-action.md) are the unit vectors towards the 12 face centres, 20 vertices and 30 edge midpoints, whose [stabilizer subgroup](../../../../../stabilizer-subgroup.md) orders are respectively $5,3,2$. Rotations about these axes exhaust the nonidentity rotations. Consequently the orbit sizes are

$$
\boxed{12,\quad20,\quad30.}
$$

## ↑ Ancestors (11)

1. [3G](../3g.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
