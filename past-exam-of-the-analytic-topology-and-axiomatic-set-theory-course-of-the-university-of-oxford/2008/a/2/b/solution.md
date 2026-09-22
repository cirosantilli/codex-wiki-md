<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Urysohn's lemma](../../../../../urysohn-s-lemma.md) states that, in a [normal space](../../../../../normal-space.md), disjoint [closed](../../../../../closed-set.md) [subsets](../../../../../subset.md) $A,B$ can be separated by a [continuous function](../../../../../continuous-function.md) $u:X\to[0,1]$ with $u=0$ on $A$ and $u=1$ on $B$.

First use the shrinking consequence of the [separation](../../../../../axiom-schema-of-specification.md) property of a [normal space](../../../../../normal-space.md): if a [closed set](../../../../../closed-set.md) $F$ lies in an [open set](../../../../../open-set.md) $G$, there is an [open](../../../../../open-set.md) $W$ with $F\subseteq W\subseteq\overline W\subseteq G$. To prove it, separate the disjoint [closed sets](../../../../../closed-set.md) $F$ and $X\setminus G$ by disjoint [open](../../../../../open-set.md) [neighborhoods](../../../../../neighbourhood-mathematics.md) $W,V$. Then $\overline W\subseteq X\setminus V\subseteq G$.

Let $D$ be the dyadic rationals in $[0,1]$. [Set](../../../../../set-split.md) $U_1=X\setminus B$, and shrink around $A$ to choose $U_0$ with $A\subseteq U_0\subseteq\overline{U_0}\subseteq U_1$. At each subsequent dyadic stage, insert between each adjacent pair $s<t$ an [open set](../../../../../open-set.md) $U_{(s+t)/2}$ such that

$$
\overline{U_s}\subseteq U_{(s+t)/2}\subseteq\overline{U_{(s+t)/2}}\subseteq U_t.
$$

The shrinking lemma applies because the first [set](../../../../../set-split.md) is [closed](../../../../../closed-set.md) and contained in the last [open set](../../../../../open-set.md). Induction gives $\overline{U_s}\subseteq U_t$ for all dyadic $s<t$. Part (a) now constructs a [continuous](../../../../../continuous-function.md) $u$. Each point of $A$ lies in $U_0$, so has value zero. Each point of $B$ lies in none of the $U_t$, so has value one. This proves the lemma.

For the embedding, let $I=C(X,[0,1])$, a [set](../../../../../set-split.md) of [continuous functions](../../../../../continuous-function.md), and define the evaluation map

$$
e:X\to\mathbb R^I,\qquad e(x)=(u(x))_{u\in I}.
$$

Every coordinate is [continuous](../../../../../continuous-function.md), so $e$ is [continuous](../../../../../continuous-function.md) in the [product topology](../../../../../product-topology.md). The [Hausdorff](../../../../../hausdorff-space.md) assumption makes singletons [closed](../../../../../closed-set.md). For distinct points, [Urysohn's lemma](../../../../../urysohn-s-lemma.md) applied to their singletons gives a coordinate with different values, so $e$ is [injective](../../../../../injective-function.md).

To check the inverse [topology](../../../../../topology-split.md), take $x\in O$ with $O$ [open](../../../../../open-set.md). Apply the lemma to $\{x\}$ and $X\setminus O$, choosing a coordinate $u$ with $u(x)=1$ and $u=0$ outside $O$. Then

$$
x\in u^{-1}((1/2,3/2))\subseteq O.
$$

This is the preimage of an [open](../../../../../open-set.md) coordinate cylinder under $e$. Thus every original [neighborhood](../../../../../neighbourhood-mathematics.md) is detected by coordinate [neighborhoods](../../../../../neighbourhood-mathematics.md), and $e^{-1}:e[X]\to X$ is [continuous](../../../../../continuous-function.md). **The evaluation map is a [topological embedding](../../../../../topological-embedding.md).**

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
