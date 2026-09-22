<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Here a [monochromatic](../../../../../monochromatic-set.md) [set](../../../../../set-split.md) must mean an infinite [homogeneous set for a colouring](../../../../../homogeneous-set-for-a-colouring.md): every singleton is a finite [monochromatic](../../../../../monochromatic-set.md) [set](../../../../../set-split.md). The requested phenomenon holds for every finite $n\ge2$. For $n=1$ it is impossible, since the colour classes of a finite [computable colouring](../../../../../computable-colouring.md) are computable and at least one is infinite. We treat this necessary qualification explicitly.

We construct a [finite-injury computable colouring of pairs](../../../../../finite-injury-computable-colouring-of-pairs.md) with no infinite computably enumerable [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md), which is stronger than the requested absence of a recursive one. Enumerate the [computably enumerable sets](../../../../../recursively-enumerable-set.md) as $W_0,W_1,\ldots$, with computable finite approximations $W_{e,s}$. Requirement $e$ seeks distinct markers $a_e,b_e\in W_e$. At stage $s$, consider indices $e\le s$ not currently assigned markers. Choose the least one, if any, for which $W_{e,s}$ has two elements outside all markers of higher-priority indices $d<e$. Assign two such elements as its markers, using a fixed least-element rule, and cancel all markers at lower-priority indices. Do nothing if no such index exists. The active markers are therefore pairwise distinct at every stage.

For $x<y$, simulate this finite construction through stage $y$ and define

$$
c(\{x,y\})=
\begin{cases}
1,&x\text{ is an active second marker }b_e\text{ at stage }y,\\
0,&\text{otherwise}.
\end{cases}
$$

In particular every active first marker has colour zero against larger points. This is a total computable [function](../../../../../function-split.md): no question about eventual enumeration or eventual stabilization is used in computing a given pair.

Induction on $e$ proves [finite injury](../../../../../finite-injury.md). Once the finitely many higher requirements have stabilized, requirement $e$ is never cancelled again. If it has markers they stay fixed. If $W_e$ is infinite, it eventually supplies two points outside the finite collection of higher markers, so it becomes eligible and is assigned markers; only finitely many higher indices could delay its assignment. Thus an infinite $W_e$ eventually has permanent distinct markers $a_e,b_e$. Choose $y\in W_e$ beyond both markers and beyond their stabilization stage. Then

$$
c(\{a_e,y\})=0,\qquad c(\{b_e,y\})=1.
$$

So $W_e$ is not homogeneous. Every infinite [recursive set](../../../../../computable-set.md) is computably enumerable, proving the desired obstruction. For $n>2$, colour an increasing $n$-tuple by the pair formed by its first two elements. Every pair from an infinite homogeneous candidate can be completed by $n-2$ larger members of that candidate, so it would give an infinite pair-homogeneous [set](../../../../../set-split.md), already ruled out.

The uncountable positive theorem is the [Erdős-Rado theorem for finite arities](../../../../../erdos-rado-theorem-for-finite-arities.md). For every infinite [cardinal](../../../../../cardinal-number.md) $\kappa$ and finite $r\ge0$, define $\beth_0(\kappa)=\kappa$ and $\beth_{r+1}(\kappa)=2^{\beth_r(\kappa)}$. Then

$$
\boxed{\beth_r(\kappa)^+\longrightarrow(\kappa^+)^{r+1}_\kappa.}
$$

The [partition relation](../../../../../partition-relation.md) means that every colouring of $(r+1)$-element [subsets](../../../../../subset.md) of the left-hand [cardinal](../../../../../cardinal-number.md) by at most $\kappa$ colours has a homogeneous [subset](../../../../../subset.md) of size $\kappa^+$. In particular, taking $\kappa=\aleph_0$ gives an uncountable [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) for every finite arity, once the domain is sufficiently large.

We prove the end-homogeneity lemma needed for induction. Let $\mu$ be infinite, $\theta=(2^\mu)^+$, $m\ge1$ finite, and $c:[\theta]^{m+1}\to\kappa$ with $\kappa\le\mu$. In a sufficiently large $H_\chi$ choose an [elementary substructure](../../../../../elementary-substructure.md) $M$ of size $2^\mu$ containing $c,\theta$ and all [ordinals](../../../../../ordinal.md) below $\mu^+$, and closed under externally given [sequences](../../../../../sequence.md) of length at most $\mu$. Here $H_\chi$ consists of [sets](../../../../../set-split.md) whose transitive closures have size below $\chi$.

To justify that closure, begin with a hull containing the indicated parameters and [ordinals](../../../../../ordinal.md). At each successor stage add every [sequence](../../../../../sequence.md) of length at most $\mu$ from the preceding stage, then take a [Skolem hull](../../../../../skolem-hull.md). There are at most $(2^\mu)^\mu=2^\mu$ such [sequences](../../../../../sequence.md). Iterate for $\mu^+$ stages and take elementary [unions](../../../../../set-union.md) at limits. The [union](../../../../../set-union.md) still has size $2^\mu$, and every [sequence](../../../../../sequence.md) of at most $\mu$ of its elements is contained in one earlier stage by regularity of $\mu^+$, so appears at the next. This proves the claimed closed [first-order model](../../../../../model-of-a-first-order-theory.md) rather than assuming its existence.

Let $\beta=\sup(M\cap\theta)<\theta$. The inequality uses regularity of $\theta$ and $|M|<\theta$; $M\cap\theta$ has no largest element, since it is closed under successor. Recursively choose increasing $x_\alpha\in M\cap\theta$ for $\alpha<\mu^+$, imposing, for every $m$-tuple $t$ of earlier points,

$$
c(t\cup\{x_\alpha\})=c(t\cup\{\beta\}).
$$

At any stage there are at most $\mu$ earlier points and constraints. Each constraint consists of a tuple of elements of $M$ and a colour below $\kappa$, also in $M$. The entire constraint code therefore belongs to $M$ by closure. The bound above the previous points belongs to $M$ as well. Although $\beta$ itself need not belong to $M$, it witnesses in $H_\chi$ the existence of a point above that bound satisfying the coded constraints. Elementarity supplies such a point inside $M$. This proves the recursion.

On the resulting [sequence](../../../../../sequence.md) $X$ of length $\mu^+$, the colour of an $(m+1)$-tuple depends only on its first $m$ entries: its last entry has the same colour contribution as $\beta$. This is the required [closed elementary-submodel construction of an end-homogeneous sequence](../../../../../closed-elementary-submodel-construction-of-an-end-homogeneous-sequence.md).

Now prove the theorem by induction on $r$. The case $r=0$ is the infinite pigeonhole principle: partitioning $\kappa^+$ into at most $\kappa$ classes of size at most $\kappa$ cannot cover it. For $r\ge1$, [set](../../../../../set-split.md) $\mu=\beth_{r-1}(\kappa)$ and apply the lemma to the colouring on $(2^\mu)^+=\beth_r(\kappa)^+$. Define a colouring of $r$-tuples from its end-homogeneous [sequence](../../../../../sequence.md) of length $\mu^+$ by their colour when completed with $\beta$. The induction hypothesis supplies a [subset](../../../../../subset.md) of size $\kappa^+$ on which this derived colouring is constant. Every original $(r+1)$-tuple from that [subset](../../../../../subset.md) has the derived colour of its first $r$ entries, and is therefore [monochromatic](../../../../../monochromatic-set.md). This completes the proof.

The unrestricted infinite-exponent situation is very different under [AC](../../../../../axiom-of-choice.md). On $[\lambda]^\omega$, choose one representative $R$ of each equivalence class modulo [finite symmetric difference](../../../../../finite-symmetric-difference.md), and colour $A$ by

$$
c(A)=|A\mathbin\triangle R|\pmod2.
$$

If $A$ is infinite and $a\in A$, deleting $a$ remains in the same equivalence class and flips the colour. Every infinite candidate [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) contains such an $A$ and $A\setminus\{a\}$ as [subsets](../../../../../subset.md), so

$$
\boxed{\lambda\nrightarrow(\omega)^\omega_2\quad\text{for every infinite cardinal }\lambda.}
$$

More generally the same argument works for [subsets](../../../../../subset.md) of any fixed infinite [cardinality](../../../../../cardinality.md): deleting one element preserves that [cardinality](../../../../../cardinality.md), so there is no unrestricted analogue with a [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) large enough to contain such [subsets](../../../../../subset.md). For the order-type-$\omega$ convention, choose $A$ in increasing order type $\omega$ and delete its first element; both [sets](../../../../../set-split.md) still have that order type. Thus the distinction from the finite-arity theorem is genuine, not merely a notational ambiguity. This argument uses [choice](../../../../../axiom-of-choice.md) of representatives and is not a claim about every definability-restricted infinite-arity colouring.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
