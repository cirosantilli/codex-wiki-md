<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The [centre of a group](../../../../../center-of-a-group.md) is $Z(G)=\{z\in G:zg=gz\text{ for every }g\in G\}$. It is a [normal subgroup](../../../../../normal-subgroup.md). For $|G|=p^r$ with $r\ge1$, let $G$ act on itself by conjugation. The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) makes the size of the conjugacy class of $g$ equal to $[G:C_G(g)]$, a power of $p$. A class has size one exactly when $g\in Z(G)$; every other class size is divisible by $p$. The [class equation](../../../../../class-equation.md) therefore gives

$$
|G|=|Z(G)|+\sum_{\text{noncentral classes}}[G:C_G(g)],
$$

so $p$ divides $|Z(G)|$. Since the identity belongs to the [centre of a group](../../../../../center-of-a-group.md), its size is a positive multiple of $p$. This proves the [nontrivial center of a finite p-group](../../../../../nontrivial-center-of-a-finite-p-group.md).

If $G/Z(G)$ is cyclic, choose a representative $a$ of a generator. Every element is $a^mz$ for an integer $m$ and $z\in Z(G)$. Any two such elements commute, since their central factors commute with everything and their remaining factors are powers of the same element. Thus $G$ is an [abelian group](../../../../../abelian-group.md), $Z(G)=G$, and **the cyclic quotient by the [centre of a group](../../../../../center-of-a-group.md) is trivial**.

For a non-[abelian group](../../../../../abelian-group.md) of order $p^3$, the [centre of a group](../../../../../center-of-a-group.md) has order $p$, $p^2$ or $p^3$ by the proved result and [Lagrange's theorem](../../../../../lagrange-s-theorem.md). The last would make the [group](../../../../../group-split.md) abelian. The middle would make $G/Z(G)$ have prime order and hence cyclic, also making $G$ abelian by the preceding argument. Therefore **its centre has order $p$**.

Finally write the given upper-unitriangular [matrix](../../../../../matrix.md) as $M(a,b,c)$. Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
M(a,b,c)M(a',b',c')=M(a+a',\,b+b'+ac',\,c+c').
$$

It commutes with every $M(a',b',c')$ exactly when $ac'=a'c$ for all $a',c'\in F$. Taking $(a',c')=(0,1)$ forces $a=0$, and taking $(1,0)$ forces $c=0$; those conditions also suffice. Thus the [centre of a group](../../../../../center-of-a-group.md) in this [Heisenberg group over a prime field](../../../../../heisenberg-group-over-a-prime-field.md) is

$$
\boxed{Z(G)=\left\{\begin{pmatrix}1&0&b\\0&1&0\\0&0&1\end{pmatrix}:b\in F\right\}.}
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
