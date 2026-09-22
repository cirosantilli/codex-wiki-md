<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

We construct a normalized positive translation-invariant functional on $C(G)$ and then represent it by a measure. The main step is a finite [matching in a graph](../../../../../matching-graph-theory.md) argument, for which we establish all the covering-net properties.

Let $V$ be an open neighbourhood of the identity in the compact [topological group](../../../../../topological-group-split.md) $G$. The sets $xV$, $x\in G$, form an open cover. Compactness supplies a finite set $F$ with $G=FV$. Among all such finite sets choose one of smallest cardinality, denoted $m(V)$. This is a [minimal left covering net of a compact group](../../../../../minimal-left-covering-net-of-a-compact-group.md). If $g\in G$, then $G=gFV$, and $gF$ has the same cardinality. Hence $gF$ is also minimal for the same $V$.

Let $F,F'$ be any two [minimal left covering nets of a compact group](../../../../../minimal-left-covering-net-of-a-compact-group.md) for $V$. They both have cardinality $m(V)$. Form a [bipartite graph](../../../../../bipartite-graph.md) by joining $x\in F$ to $y\in F'$ whenever $xV\cap yV\ne\varnothing$. For a subset $S\subseteq F$, let $N(S)$ be its set of neighbours. Every point of $SV$ lies in some $yV$ with $y\in F'$; that $y$ is a neighbour of a member of $S$. Therefore

$$
SV\subseteq N(S)V,
$$

and $(F\setminus S)\cup N(S)$ is still a left covering set. By minimality,

$$
m(V)\leq |(F\setminus S)\cup N(S)|\leq m(V)-|S|+|N(S)|.
$$

Thus $|N(S)|\geq|S|$. [Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) gives a [bijection](../../../../../bijection.md) $\pi:F\to F'$ with $xV\cap\pi(x)V\ne\varnothing$ for every $x$. If $xv=\pi(x)v'$ at an intersection point, then

$$
\boxed{x^{-1}\pi(x)=vv'^{-1}\in VV^{-1}.}
$$

This proves the [matching minimal covering nets of a compact group](../../../../../matching-minimal-covering-nets-of-a-compact-group.md) property, including the estimate needed below.

For a continuous complex-valued function $f$ on $G$, define

$$
I_F(f)=\frac1{|F|}\sum_{x\in F}f(x),\qquad
\omega_f(W)=\sup\{|f(xw)-f(x)|:x\in G,\ w\in W\}.
$$

Continuity and compactness imply $\omega_f(W)\to0$ as identity neighbourhoods $W$ shrink. Here is the uniformity argument: continuity of $(x,w)\mapsto f(xw)-f(x)$ at each $(x,e)$ gives a product neighbourhood where its absolute value is small; finitely many of the first-coordinate neighbourhoods cover $G$, and intersecting the corresponding second-coordinate neighbourhoods gives one $W$ that works for every $x$.

Matched pairs therefore give

$$
|I_F(f)-I_{F'}(f)|\leq\omega_f(VV^{-1}).
$$

In particular, with $F'=gF$,

$$
\boxed{|I_F(f\circ L_g)-I_F(f)|\leq\omega_f(VV^{-1}),\qquad L_g(x)=gx.}
$$

The estimate holds for every $g\in G$; no commutativity of $G$ is being assumed.

Direct the open identity neighbourhoods by reverse inclusion and choose a [minimal left covering net of a compact group](../../../../../minimal-left-covering-net-of-a-compact-group.md) $F_V$ for each. The values $I_{F_V}(f)$ lie in the closed complex disk of radius $\|f\|_\infty$. The [Tychonoff theorem](../../../../../tychonoff-s-theorem.md) makes the product of these disks over all $f\in C(G)$ compact. Consequently the [net](../../../../../net-mathematics.md) of vectors $(I_{F_V}(f))_{f\in C(G)}$ has a convergent [subnet](../../../../../subnet-of-a-net.md). Call its coordinatewise limit $I(f)$. Since each finite average is linear, positive on nonnegative real functions, and equal to one at the constant function one, the limit satisfies

$$
I(\alpha f+\beta h)=\alpha I(f)+\beta I(h),\qquad I(f)\geq0\ (f\geq0),\qquad I(1)=1,
$$

and $|I(f)|\leq\|f\|_\infty$. Thus $I$ is a bounded [positive linear functional](../../../../../positive-linear-functional.md).

Given an identity neighbourhood $W$, continuity of multiplication and inversion supplies a sufficiently small $V$ with $VV^{-1}\subseteq W$. The translation estimate consequently tends to zero along the [subnet](../../../../../subnet-of-a-net.md). For every $f\in C(G)$ and every $g\in G$,

$$
\boxed{I(f\circ L_g)=I(f).}
$$

The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) now represents $I$ by a regular positive [Borel measure](../../../../../borel-measure.md) $\mu$ with $\mu(G)=1$. The preceding equality and uniqueness in that representation imply that the pushforward under every left translation equals $\mu$. Hence

$$
\boxed{\mu(gE)=\mu(E)\quad\hbox{for every Borel set }E\subseteq G.}
$$

This is the required normalized [Haar measure](../../../../../haar-measure.md). It is nonzero because its total mass is one. In fact every nonempty open set has positive measure: its left translates cover $G$, a finite subcover exists, and a zero measure for that open set would force $\mu(G)=0$.

For completeness, the constructed probability measure is also right invariant. Apply [Fubini's theorem](../../../../../fubini-s-theorem.md) to $f(x^{-1}y)$ with both variables distributed according to $\mu$. Integrating first in $y$ gives $\int f\,d\mu$ by left invariance. Integrating first in $x$ and substituting $x=yz$ gives $\int f(z^{-1})\,d\mu(z)$. Thus $\mu$ is invariant under inversion. Inversion turns a right translation into a left translation, so right invariance follows. This last observation is not needed for the existence of a left [Haar measure](../../../../../haar-measure.md), but confirms the usual two-sided normalization for [compact groups](../../../../../compact-group.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
