<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Symmetrization for an arbitrary real coefficient.** Among [graphs](../../../../../graph-split.md) maximizing $f(G)=e(G)-c k_3(G)$, choose one maximizing

$$
Q(G)=\sum_{x\in V(G)}d(x)^2.
$$

For a [vertex](../../../../../vertex-graph-theory.md) $x$, put $L(x)=d(x)-c e(G[N(x)])$. This is the contribution of [edges](../../../../../edge-of-a-graph.md) and [triangles in a graph](../../../../../triangle-in-a-graph.md) containing $x$. If $u,v$ are nonadjacent, [Zykov symmetrization](../../../../../zykov-symmetrization.md) replacing $u$ by a clone of $v$ changes $f$ by $L(v)-L(u)$; the opposite replacement changes it by $L(u)-L(v)$. Maximality implies $L(u)=L(v)$, so both changes preserve $f$.

Let $S=N(v)\setminus N(u)$ and $T=N(u)\setminus N(v)$. In the first replacement the [vertex degrees](../../../../../degree-graph-theory.md) in $S$ increase by one and those in $T$ decrease by one; in the opposite replacement these changes reverse. The changes to $d(u)^2+d(v)^2$ cancel when the two replacements are added. Since $(d+1)^2+(d-1)^2-2d^2=2$,

$$
\Delta_{u\gets v}Q+\Delta_{v\gets u}Q=2(|S|+|T|).
$$

If the two [vertex neighbourhoods](../../../../../vertex-neighbourhood.md) differ, one replacement increases $Q$, a contradiction. Thus every pair of nonadjacent [vertices](../../../../../vertex-graph-theory.md) has the same [vertex neighbourhood](../../../../../vertex-neighbourhood.md). Nonadjacency, with equality allowed, is an [equivalence relation](../../../../../equivalence-relation.md): if $u$ and $v$ are nonadjacent and $v$ and $w$ are nonadjacent, their identical [vertex neighbourhoods](../../../../../vertex-neighbourhood.md) forbid $uw$ as well. Its classes are [independent sets](../../../../../independent-set-graph-theory.md) and every cross-class [edge](../../../../../edge-of-a-graph.md) is present. Therefore

$$
\boxed{\text{some maximizer of }e(G)-c k_3(G)\text{ is complete multipartite}.}
$$

This [edge-triangle symmetrization](../../../../../edge-triangle-symmetrization.md) works for either sign of $c$.

**The exact supporting line.** For $n\geq3$, write

$$
e_2=e(T_2(n)),\quad e_3=e(T_3(n)),\quad t_3=k_3(T_3(n)),\quad c_*=(e_3-e_2)/t_3.
$$

We prove the [triangle support line between bipartite and tripartite Turan graphs](../../../../../triangle-support-line-between-bipartite-and-tripartite-turan-graphs.md) by maximizing $e-c_*k_3$. First $c_*\geq2/n$. For $n=3,4,5$, its values are respectively $1,1/2,1/2$. For $n\geq6$, the exact balancing of the [Turán graph](../../../../../turan-graph.md) gives $e_3\geq n^2/3-1/3$, while $e_2\leq n^2/4$ and the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) gives $t_3\leq n^3/27$. Hence

$$
n(e_3-e_2)-2t_3\geq\frac{n^3}{108}-\frac n3\geq0.
$$

By [edge-triangle symmetrization](../../../../../edge-triangle-symmetrization.md) a maximizing [graph](../../../../../graph-split.md) can be taken [complete multipartite graph](../../../../../complete-multipartite-graph.md); among such maximizers use one with the fewest nonempty parts. If there are at least four parts, let $a,b$ be the two smallest sizes. Then $a+b\leq n/2$. Merging them loses $ab$ [edges](../../../../../edge-of-a-graph.md) and $ab(n-a-b)$ [triangles in a graph](../../../../../triangle-in-a-graph.md), so the objective changes by

$$
ab\{c_*(n-a-b)-1\}\geq0.
$$

This contradicts the choice of the number of parts. Thus at most three parts remain.

For three part sizes $a\geq b\geq d>0$, the objective is

$$
ad(1-c_*b)+b(a+d).
$$

If $1-c_*b\leq0$, merging the parts of sizes $a,d$ does not decrease it, again contradicting minimality. If $1-c_*b>0$ and $a-d\geq2$, transferring one [vertex](../../../../../vertex-graph-theory.md) from the largest to the smallest part raises $ad$ by $a-d-1>0$ and strictly increases the objective. Thus a three-part maximizer has all sizes differing by at most one, and is $T_3(n)$. A maximizer with at most two parts has objective at most $e_2$, since it has no [triangles in a graph](../../../../../triangle-in-a-graph.md) and the [Mantel theorem](../../../../../mantel-theorem.md) bounds its [edges](../../../../../edge-of-a-graph.md). Finally,

$$
e(T_3(n))-c_*k_3(T_3(n))=e_2.
$$

Therefore every [graph](../../../../../graph-split.md) satisfies $e(G)-c_*k_3(G)\leq e_2$. At the prescribed [edge](../../../../../edge-of-a-graph.md) count this gives

$$
\boxed{k_3(G)\geq\theta k_3(T_3(n)).}
$$

For $n\leq2$, the conclusion is simply the nonnegative lower bound zero. All rounding in the [Turán graphs](../../../../../turan-graph.md) has been retained.

**One edge above the bipartite threshold.** Write $n=2m$. We prove the [Triangle lower bound one edge above the Mantel threshold](../../../../../triangle-lower-bound-one-edge-above-the-mantel-threshold.md) by induction on $m\geq2$, allowing at least $m^2+1$ [edges](../../../../../edge-of-a-graph.md). For $m=2$, five [edges](../../../../../edge-of-a-graph.md) on four [vertices](../../../../../vertex-graph-theory.md) give two [triangles in a graph](../../../../../triangle-in-a-graph.md), and adding [edges](../../../../../edge-of-a-graph.md) preserves this bound.

We will also use the following consequence of an inductive bound: on $2a$ [vertices](../../../../../vertex-graph-theory.md), at least $a^2+q$ [edges](../../../../../edge-of-a-graph.md), for an integer $q\geq1$, force at least $a+q-1$ [triangles in a graph](../../../../../triangle-in-a-graph.md). Delete surplus [edges](../../../../../edge-of-a-graph.md) first to leave exactly $a^2+q$. Repeatedly delete an [edge](../../../../../edge-of-a-graph.md) in a [triangle in a graph](../../../../../triangle-in-a-graph.md) until $a^2+1$ [edges](../../../../../edge-of-a-graph.md) remain. The [Mantel theorem](../../../../../mantel-theorem.md) guarantees such a [triangle in a graph](../../../../../triangle-in-a-graph.md) at every step; each deletion destroys at least one distinct [triangle in a graph](../../../../../triangle-in-a-graph.md). Apply the inductive bound to the remaining [graph](../../../../../graph-split.md).

Now take exactly $m^2+1$ [edges](../../../../../edge-of-a-graph.md). If every [edge](../../../../../edge-of-a-graph.md) lies in a [triangle in a graph](../../../../../triangle-in-a-graph.md), the [edge-triangle incidence bound](../../../../../edge-triangle-incidence-bound.md) gives $3k_3(G)\geq m^2+1$. This is at least $3m$ for $m\geq3$; the base case was handled separately.

Otherwise choose an [edge](../../../../../edge-of-a-graph.md) $uv$ in no [triangle in a graph](../../../../../triangle-in-a-graph.md). Its endpoints have disjoint [vertex neighbourhoods](../../../../../vertex-neighbourhood.md), so $d(u)+d(v)\leq2m$. Deleting $u,v$ removes exactly $d(u)+d(v)-1$ [edges](../../../../../edge-of-a-graph.md) and leaves at least $(m-1)^2+1$ [edges](../../../../../edge-of-a-graph.md). If $d(u)+d(v)\leq2m-1$, it leaves at least $(m-1)^2+2$ [edges](../../../../../edge-of-a-graph.md), and the strengthened inductive bound gives at least $m$ [triangles in a graph](../../../../../triangle-in-a-graph.md) already.

If $d(u)+d(v)=2m$, induction gives at least $m-1$ [triangles in a graph](../../../../../triangle-in-a-graph.md) after deletion. There must be an additional [triangle in a graph](../../../../../triangle-in-a-graph.md) containing $u$ or $v$. Otherwise both $N(u)$ and $N(v)$ are [independent sets](../../../../../independent-set-graph-theory.md); since they are disjoint and cover all [vertices](../../../../../vertex-graph-theory.md), $G$ would be [bipartite graph](../../../../../bipartite-graph.md), contradicting $e(G)>m^2$ by the [Mantel theorem](../../../../../mantel-theorem.md). Hence

$$
\boxed{k_3(G)\geq m=n/2.}
$$

The bound is sharp: add one internal [edge](../../../../../edge-of-a-graph.md) to one class of the [complete bipartite graph](../../../../../complete-bipartite-graph.md) $K_{m,m}$. Its [triangles in a graph](../../../../../triangle-in-a-graph.md) are precisely that [edge](../../../../../edge-of-a-graph.md) together with each of the $m$ [vertices](../../../../../vertex-graph-theory.md) in the other class.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
