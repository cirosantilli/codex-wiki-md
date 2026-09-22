<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

If $\mathcal B$ is a [countable](../../../../countable-set.md) [topological basis](../../../../basis-of-a-topology.md) of $X$, then $\{B\cap Y:B\in\mathcal B\}$ is a [countable](../../../../countable-set.md) [topological basis](../../../../basis-of-a-topology.md) of the subspace $Y$. Indeed every subspace-[open neighborhood](../../../../open-neighbourhood.md) is $Y\cap U$ for an open $U$ of $X$, and a suitable basic set lies between its [point](../../../../point-geometry.md) and $U$. This proves the first assertion.

**[Urysohn's metrisation theorem](../../../../urysohn-s-metrization-theorem.md):** every [second-countable space](../../../../second-countable-space.md) that is also a [T3 space](../../../../t3-space.md) is a [metrizable space](../../../../metrizable-space.md). Here [regularity of a topological space](../../../../regular-topological-space.md) allows a [neighborhood](../../../../neighbourhood-mathematics.md) of a [point](../../../../point-geometry.md) to be shrunk to an [open neighborhood](../../../../open-neighbourhood.md) whose [closure](../../../../closure-topology.md) is still inside the original one.

We first prove the separation facts needed in a complete proof. [Second countability](../../../../second-countable-space.md) implies the [Lindelöf](../../../../lindelof-space.md) property: for each basic set contained in some member of an [open cover](../../../../open-cover.md) choose one such member; these countably many members cover. In particular closed subspaces are [Lindelöf](../../../../lindelof-space.md). For disjoint [closed sets](../../../../closed-set.md) $F,G$, [regularity of a topological space](../../../../regular-topological-space.md) and this property give open covers $F\subseteq\bigcup_nU_n$, $G\subseteq\bigcup_nV_n$ with $\overline U_n\cap G=\varnothing$ and $\overline V_n\cap F=\varnothing$. Define

$$
U=\bigcup_n\left(U_n\setminus\bigcup_{j\leq n}\overline V_j\right),\qquad V=\bigcup_n\left(V_n\setminus\bigcup_{j\leq n}\overline U_j\right).
$$

These sets are open and contain $F,G$ respectively. They are disjoint: if a [point](../../../../point-geometry.md) belonged to a term indexed by $n$ in the first union and by $m$ in the second, the term with the larger index would have removed the [closure](../../../../closure-topology.md) of the other covering set. Thus the space is a [normal space](../../../../normal-space.md).

For completeness, [Urysohn's lemma](../../../../urysohn-s-lemma.md) supplies [continuous](../../../../continuous-function.md) separating functions in a [normal topological space](../../../../normal-space.md). Its construction is as follows. Given disjoint closed $F,G$, choose [open sets](../../../../open-set.md) $O_r$ for dyadic $r\in[0,1]$, with $F\subseteq O_0$, $O_1=X\setminus G$, and $\overline O_r\subseteq O_s$ whenever $r<s$. Start by shrinking a [neighborhood](../../../../neighbourhood-mathematics.md) of $F$ inside $X\setminus G$, and insert the successive dyadic sets by the [closed-neighborhood shrinking in a normal space](../../../../closed-neighborhood-shrinking-in-a-normal-space.md). Define

$$
f(x)=\inf\bigl(\{r:x\in O_r\}\cup\{1\}\bigr).
$$

Then $f=0$ on $F$, $f=1$ on $G$, and $0\leq f\leq1$. The identities $\{f<a\}=\bigcup_{r<a}O_r$ and $\{f>a\}=\bigcup_{a<r<1}(X\setminus\overline O_r)$ prove [continuity](../../../../continuous-function.md) for $0<a<1$, with the endpoint cases immediate.

Let $\{B_n\}$ be a [countable](../../../../countable-set.md) [topological basis](../../../../basis-of-a-topology.md). For each pair $(n,m)$ with $\overline B_n\subseteq B_m$, choose a [continuous function](../../../../continuous-function.md) $f_{nm}:X\to[0,1]$ equal to one on $\overline B_n$ and zero outside $B_m$. These form a [countable](../../../../countable-set.md) family. Given $x\in O$ open, choose $B_m$ with $x\in B_m\subseteq O$, shrink a [neighborhood](../../../../neighbourhood-mathematics.md) of $x$ inside $B_m$, and then choose $B_n$ inside that smaller [neighborhood](../../../../neighbourhood-mathematics.md). Thus

$$
x\in\{f_{nm}>1/2\}\subseteq B_m\subseteq O.
$$

Consequently these functions generate the original topology. They also separate distinct [points](../../../../point-geometry.md): use the $T_1$ [open set](../../../../open-set.md) $X\setminus\{y\}$ when $x\ne y$. Enumerate them as $f_j$, padding by zero functions if necessary. The map $x\mapsto(f_j(x))_j$ is a [topological embedding](../../../../topological-embedding.md) into the [countable](../../../../countable-set.md) cube. Pulling back its [metric](../../../../metric.md), or directly using

$$
\boxed{d(x,y)=\sum_{j=1}^{\infty}2^{-j}|f_j(x)-f_j(y)|,}
$$

gives a compatible [metric](../../../../metric.md). The fact that the functions distinguish distinct points proves positivity for distinct [points](../../../../point-geometry.md), the [triangle inequality](../../../../triangle-inequality.md) is termwise, and the uniformly bounded tails show that this [metric](../../../../metric.md) induces exactly the topology generated by the coordinates. Empty and singleton spaces are trivially [metrizable spaces](../../../../metrizable-space.md). This proves the theorem.

For the application, a [separable](../../../../separable-topological-space.md) [metric space](../../../../metric-space.md) has a [countable](../../../../countable-set.md) [topological basis](../../../../basis-of-a-topology.md) consisting of balls with rational positive radii about a [countable](../../../../countable-set.md) [dense](../../../../dense-set.md) set, and it is a [T3 space](../../../../t3-space.md). The given product theorems make a [countable](../../../../countable-set.md) product of these spaces [second countable](../../../../second-countable-space.md) and a [T3 space](../../../../t3-space.md). Urysohn's theorem makes it a [metrizable space](../../../../metrizable-space.md). Finally every [second countable](../../../../second-countable-space.md) space is [separable](../../../../separable-topological-space.md): choose a [point](../../../../point-geometry.md) from each nonempty basic [open set](../../../../open-set.md); the resulting [countable](../../../../countable-set.md) set meets every nonempty [open set](../../../../open-set.md). Hence the product is **[separable](../../../../separable-topological-space.md) and a [metrizable space](../../../../metrizable-space.md)**.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
