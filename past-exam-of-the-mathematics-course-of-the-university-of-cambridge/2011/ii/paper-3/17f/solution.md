<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

The [Turán graph](../../../../../turan-graph.md) $T_r(n)$ is the complete $r$-partite graph whose vertex-class sizes differ by at most one; empty classes are allowed when $r>n$. Its edge count is $t_r(n)=\frac12(n^2-\sum_{i=1}^rn_i^2)$. [Turan theorem](../../../../../turan-s-theorem.md) states that every $n$-vertex graph containing no $K_{r+1}$ has at most $t_r(n)$ edges.

Here is a symmetrization proof, including the equality case. Let $G$ be any $K_{r+1}$-free graph maximizing the edge count. If nonadjacent $u,v$ have unequal degrees, replace the lower-degree vertex by a twin of the higher-degree vertex: this increases edges and cannot create a forbidden clique, since any new clique containing the twin corresponds to an old clique containing its model. Thus all nonadjacent pairs have equal degrees.

If such $u,v$ had distinct neighbourhoods, choose $w\in N(u)\setminus N(v)$ (their equal degrees ensure such a vertex exists), and clone $v$ onto $u$. The new graph has the same maximum number of edges and is still clique-free. Originally $w$ and $v$ were nonadjacent, so $d(w)=d(v)$. After cloning, $w$ loses precisely its edge to $u$, while $v$ keeps its degree. They remain nonadjacent but now have different degrees, contradicting the preceding necessary property of every extremal graph. Hence nonadjacent vertices have identical neighbourhoods.

Nonadjacency together with equality is therefore an equivalence relation, making $G$ complete multipartite. It has at most $r$ classes, otherwise choosing one vertex from each of $r+1$ classes gives a clique. For fixed total size, $\sum n_i^2$ is minimized by $r$ classes balanced as equally as possible: splitting a nontrivial class when fewer than $r$ classes are used adds edges, and moving a vertex from a class of size at least two greater than another also adds edges. Thus every extremal graph is $T_r(n)$, up to isomorphism. This proves both the bound and its equality characterization. In particular

$$
\boxed{\operatorname{ex}(K_3;n)=t_2(n)=\lfloor n^2/4\rfloor.}
$$

For the bipartite assertion, take a maximum [matching in a graph](../../../../../matching-graph-theory.md) of $a$ edges. No edge joins two unmatched vertices. Let $U$ be its $2a$ endpoints. For each matched pair $uv$, both $u$ and $v$ cannot have neighbours outside $U$: those two neighbours lie in opposite vertex classes and would replace $uv$ by two disjoint edges, increasing the matching. Thus at most $n-a$ edges from this pair lead outside $U$, giving $|F|\leq a(n-a)$. There are at most $a^2$ edges within $U$. Consequently

$$
e(G)\leq a^2+a(n-a)=an.
$$

If $e(G)>(k-1)n$, necessarily $a\geq k$.

Finally let $A,B,C$ be the three classes of the triangle-free graph. If $m=e(A,B)=0$, the desired bound is immediate. Otherwise set $k=\lceil m/n\rceil$. The preceding result gives $k$ disjoint $AB$ edges. For each edge $uv$, the $C$-neighbourhoods of its endpoints are disjoint, or there would be a triangle, so $d_C(u)+d_C(v)\leq n$. The other $2(n-k)$ vertices of $A\cup B$ each have at most $n$ neighbours in $C$. Hence

$$
e(A,C)+e(B,C)\leq kn+2(n-k)n=2n^2-kn.
$$

Since $m\leq kn$,

$$
\boxed{e(H)\leq2n^2.}
$$

Equality is attained by retaining every $AC$ and $BC$ edge and no $AB$ edges.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
