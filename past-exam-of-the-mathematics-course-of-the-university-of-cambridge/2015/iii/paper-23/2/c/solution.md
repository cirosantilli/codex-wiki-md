<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [torsion-free divisible Abelian group](../../../../../../torsion-free-divisible-abelian-group.md) is naturally a [vector space over the rational numbers](../../../../../../vector-space-over-the-rational-numbers.md): for $m\in\mathbb Z$ and $n>0$, define $(m/n)a$ as the unique $b$ with $nb=ma$. Divisibility supplies existence and torsion-freeness supplies uniqueness.

In the usual group [first-order language](../../../../../../first-order-language.md) $\{+, -,0\}$, a model $A$ of the universal part of [DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md) is a [torsion-free group](../../../../../../torsion-free-group.md) which is Abelian. If the language instead uses only $\{+,0\}$, a [substructure](../../../../../../substructure-of-a-first-order-structure.md) can be merely a [torsion-free cancellative commutative monoid](../../../../../../torsion-free-cancellative-commutative-monoid.md). Handle this convention by first taking its [Grothendieck group](../../../../../../grothendieck-group.md) $G(A)$: its elements are formal differences $a-b$, with

$$
a-b=a'-b'\quad\Longleftrightarrow\quad a+b'=a'+b.
$$

The [cancellative commutative monoid](../../../../../../cancellative-commutative-monoid.md) condition makes $A\to G(A)$ injective. If $n(a-b)=0$, then $na=nb$, and torsion-freeness gives $a=b$; hence $G(A)$ is a [torsion-free abelian group](../../../../../../torsion-free-abelian-group.md). In the full group language simply take $G(A)=A$.

For $A\ne\{0\}$ form its [rational divisible hull](../../../../../../rational-divisible-hull.md)

$$
P=G(A)\otimes_{\mathbb Z}\mathbb Q.
$$

Concretely its elements are fractions $g/n$ with $n>0$, where $g/n=h/m$ if $mg=nh$. The canonical embedding of $A$ into $P$ is injective, and $P$ is nontrivial, divisible, Abelian and torsion-free, so it satisfies [DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md).

Let $j:A\to N$ be any [structure embedding](../../../../../../structure-embedding.md) into a model of [DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md). Extend it first to formal differences if necessary. Its unique extension to the [rational divisible hull](../../../../../../rational-divisible-hull.md) sends $g/n$ to the unique element $b\in N$ with $nb=j(g)$. This is a [group homomorphism](../../../../../../group-homomorphism.md) fixing the given copy of $A$. It is injective: an element mapped to zero has $j(g)=0$, hence $g=0$. Thus every embedding into a [DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md) model factors through $P$.

The zero case must be treated separately: its [rational divisible hull](../../../../../../rational-divisible-hull.md) is zero and does not satisfy [DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md). Instead choose $P=(\mathbb Q,+)$. Given any nontrivial [DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md) model $N$, choose $b\ne0$; the map $q\mapsto qb$ embeds $P$ into $N$ over zero. Therefore **[DAG](../../../../../../theory-of-nontrivial-torsion-free-divisible-abelian-groups.md) has [algebraically prime models](../../../../../../algebraically-prime-extension.md), including over the trivial base.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
