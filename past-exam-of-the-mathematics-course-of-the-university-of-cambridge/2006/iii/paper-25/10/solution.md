<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

For an infinite cardinal $\rho$ put $\beth_0(\rho)=\rho$ and $\beth_{n+1}(\rho)=2^{\beth_n(\rho)}$. The [Erdős-Rado theorem for finite arities](../../../../../erdos-rado-theorem-for-finite-arities.md) is

$$
\boxed{\beth_n(\rho)^+\longrightarrow(\rho^+)^{n+1}_\rho\qquad(n<\omega).}
$$

The [partition relation](../../../../../partition-relation.md) requires a homogeneous [subset](../../../../../subset.md) of order type $\rho^+$ for every coloring of $(n+1)$-element [subsets](../../../../../subset.md) by at most $\rho$ colors. In particular it gives [uncountable](../../../../../uncountable-set.md) [homogeneous sets](../../../../../homogeneous-set-for-a-colouring.md). The case $n=0$ is the infinite pigeonhole principle: a [union](../../../../../set-union.md) of $\rho$ [sets](../../../../../set-split.md) each of size at most $\rho$ cannot have size $\rho^+$.

We give the induction step by a [closed elementary-submodel construction of an end-homogeneous sequence](../../../../../closed-elementary-submodel-construction-of-an-end-homogeneous-sequence.md). Let $\mu$ be infinite, $\theta=(2^\mu)^+$, and $c:[\theta]^{r+1}\to\rho$ with $\rho\le\mu$. Choose a sufficiently large regular $\chi$ and an elementary submodel $M\prec H_\chi$ with $c,\theta\in M$, all [ordinals](../../../../../ordinal.md) below $\mu^+$ in $M$, $|M|=2^\mu$, and closure under externally given [sequences](../../../../../sequence.md) of length at most $\mu$. To construct it, take $\mu^+$ successive elementary Skolem-hull closures, at each step including all such [sequences](../../../../../sequence.md) from the preceding stage. [Cardinality](../../../../../cardinality.md) stays $2^\mu$ because $(2^\mu)^\mu=2^\mu$. In the final [union](../../../../../set-union.md) every [sequence](../../../../../sequence.md) of length at most $\mu$ has all its entries in some earlier stage, by regularity of $\mu^+$, and so was included at the next stage.

Put $\beta=\sup(M\cap\theta)$. Regularity of $\theta$ gives $\beta<\theta$, and $\beta\notin M$ since otherwise its successor would contradict the definition of the supremum. Recursively, for $\alpha<\mu^+$ choose $x_\alpha\in M\cap\theta$ above all earlier $x_\xi$ and satisfying

$$
c(\{x_{\xi_1},\ldots,x_{\xi_r},x_\alpha\})
=c(\{x_{\xi_1},\ldots,x_{\xi_r},\beta\})\qquad(\xi_1<\cdots<\xi_r<\alpha).
$$

There are at most $\mu$ constraints. Their parameters and their colors belong to $M$, and closure puts their complete code in $M$. The point $\beta$ witnesses their simultaneous satisfiability in $H_\chi$; elementarity supplies a witness in $M$. This gives an increasing end-homogeneous [sequence](../../../../../sequence.md) of length $\mu^+$: on it, the color of an $(r+1)$-tuple depends only on the first $r$ entries.

For the induction from arity $n$ to $n+1$, take $\mu=\beth_{n-1}(\rho)$ and $r=n$. Color the $n$-tuples of the resulting [sequence](../../../../../sequence.md) by their common color with a later point, equivalently by their color with $\beta$. Its index order has type $\mu^+=\beth_{n-1}(\rho)^+$, so the induction hypothesis supplies a homogeneous index [set](../../../../../set-split.md) of type $\rho^+$. The original $(n+1)$-tuples on those indices have that same color. This completes the proof without substituting the theorem's name for its induction.

A useful [ordinal partition-bound function](../../../../../ordinal-partition-bound-function.md) is

$$
f(\alpha)=\min\{\gamma\ge\alpha:\ \gamma\longrightarrow(\alpha)^2_\nu\text{ for every nonzero cardinal }\nu<\alpha\}.
$$

It is total: choose an infinite cardinal $\rho\ge|\alpha|$ with $\rho^+>\alpha$; the pairs case supplies $(2^\rho)^+$ with the required homogeneous order type for all these color numbers. It is nondecreasing and satisfies $f(\alpha)\ge\alpha$. Start iterating $f$ and take a supremum $\kappa$ at a limit stage. If the increasing iterates do not attain that supremum, then for every $\alpha<\kappa$ some iterate $a_\xi$ satisfies $\alpha\le a_\xi<\kappa$, and

$$
f(\alpha)\le f(a_\xi)=a_{\xi+1}<\kappa.
$$

If the iterates have already stabilized, their supremum is a fixed point directly. Thus the relevant nontrivial case is an [uncountable](../../../../../uncountable-set.md) cardinal $\kappa$ closed below itself under $f$.

Such closure implies that $\kappa$ is a strong limit. Suppose $\lambda<\kappa$ is infinite and $\kappa\le2^\lambda$. Take distinct binary strings of length $\lambda$, indexed in order by $\kappa$, and color a pair by its first differing coordinate. No three strings are homogeneous: three bits cannot be pairwise different at the same coordinate. Closure would give $f(\lambda+1)<\kappa$, and its restriction would have a homogeneous [subset](../../../../../subset.md) of order type $\lambda+1$ in $\lambda$ colors, a contradiction. Hence $2^\lambda<\kappa$; finite exponents are harmless for an [uncountable](../../../../../uncountable-set.md) $\kappa$.

Use the usual [tree property](../../../../../tree-property.md): every [set-theoretic tree](../../../../../set-theoretic-tree.md) of height $\kappa$ with nonempty levels of [cardinality](../../../../../cardinality.md) below $\kappa$ has a cofinal branch. For an [uncountable](../../../../../uncountable-set.md) cardinal satisfying this all-[set-theoretic trees](../../../../../set-theoretic-tree.md) convention, $\kappa$ must be regular. If it were singular with [cofinality](../../../../../cofinality.md) $\tau<\kappa$, attach to one root $\tau$ chains whose lengths increase cofinally to $\kappa$. Every level has at most $\tau$ nodes, the height is $\kappa$, and no branch is cofinal. This contradiction proves regularity. Combined with the preceding closure argument it proves that the cardinal under discussion is strongly inaccessible.

For any $c:[\kappa]^2\to\nu$, $0<\nu<\kappa$, make a separated [set-theoretic tree](../../../../../set-theoretic-tree.md) of [functions](../../../../../function-split.md). Its level $\alpha$ consists of the [functions](../../../../../function-split.md) $t:\alpha\to\nu$ realized as $t(\xi)=c(\{\xi,\beta\})$ for some $\beta\ge\alpha$, with $\beta<\kappa$. Order these [functions](../../../../../function-split.md) by restriction. Levels are nonempty and have size at most $\nu^{|\alpha|}<\kappa$, using the strong-limit property. The [tree property](../../../../../tree-property.md) gives a branch $b:\kappa\to\nu$. Recursively select $x_\eta$ for $\eta<\kappa$, larger than all earlier selections, whose coloring [function](../../../../../function-split.md) agrees with $b$ through a level above those earlier selections; regularity allows that level to remain below $\kappa$, and its node has a realizing point. Then $c(\{x_\xi,x_\eta\})=b(x_\xi)$ for $\xi<\eta$. One of the fewer-than-$\kappa$ colors occurs on $\kappa$ selected points, by regularity. These points are homogeneous, proving $\kappa\to(\kappa)^2_\nu$ for every $\nu<\kappa$. Consequently

$$
\boxed{\kappa\text{ closed below itself under }f\ +\ \mathrm{TP}(\kappa)\quad\Longrightarrow\quad f(\kappa)=\kappa.}
$$

A strictly increasing [countable](../../../../../countable-set.md) iteration has a supremum of [countable](../../../../../countable-set.md) [cofinality](../../../../../cofinality.md), so it cannot meet this regular [set-theoretic tree](../../../../../set-theoretic-tree.md)-property condition; no continuity of $f$ has been assumed.

The final printed assertion needs its convention specified. The usual [tree property](../../../../../tree-property.md) alone does not imply strong inaccessibility; it can consistently hold at [successor cardinals](../../../../../successor-cardinal.md). In the argument just given, strong inaccessibility follows from [function](../../../../../function-split.md) closure together with that [set-theoretic tree](../../../../../set-theoretic-tree.md) property. There is also a stronger [branching form of the tree property](../../../../../branching-form-of-the-tree-property.md) for which the assertion holds literally: require a cofinal branch in every separated rooted height-$\kappa$ [set-theoretic tree](../../../../../set-theoretic-tree.md) whose nodes each have fewer than $\kappa$ immediate successors, without restricting level sizes. The singular-chain example proves regularity under this convention too. If $2^\lambda\ge\kappa$ for $\lambda<\kappa$, take the full binary [set-theoretic tree](../../../../../set-theoretic-tree.md) through level $\lambda$, choose $\kappa$ distinct nodes on that level, and attach to its $\xi$th chosen node a chain of length $\xi$, for $\xi<\kappa$. It has height $\kappa$ and at most two successors per node, but every branch has length below $\kappa$. Thus this branching property implies the strong-limit condition and hence strong inaccessibility. At a [strongly inaccessible cardinal](../../../../../strongly-inaccessible-cardinal.md) it agrees, for separated [set-theoretic trees](../../../../../set-theoretic-tree.md), with the usual level-size convention: regularity bounds the [union](../../../../../set-union.md) of fewer than $\kappa$ successor [sets](../../../../../set-split.md), and strong-limit arithmetic bounds the possible predecessor [sequences](../../../../../sequence.md) at limit levels.

## ↑ Ancestors (10)

1. [10](../10.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
