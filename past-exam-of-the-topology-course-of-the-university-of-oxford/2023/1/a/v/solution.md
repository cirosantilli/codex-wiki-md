<h1 id="1/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The intended hypothesis is that $A$ is not [connected](../../../../../connected-space.md). The original PDF has the same grammatical ambiguity as the transcription. If only $X$ were assumed not [connected](../../../../../connected-space.md), the assertion would fail for the [discrete space](../../../../../discrete-space.md) $X=\{0,1\}$ with its usual [metric](../../../../../metric.md) and the [closed subset](../../../../../closed-set.md) $A=\{0\}$: two disjoint sets cannot both meet that [singleton](../../../../../singleton-mathematics.md).

Under the intended reading, choose a [separation of a topological space](../../../../../separation-of-a-topological-space.md) $A=B\sqcup C$. Both $B$ and $C$ are nonempty and [closed](../../../../../closed-set.md) in $A$, because each is the complement of the other relatively [open](../../../../../open-set.md) part. Since $A$ is [closed](../../../../../closed-set.md) in $X$, both are [closed](../../../../../closed-set.md) in $X$.

For a nonempty [subset](../../../../../subset.md) $F$ of the [metric space](../../../../../metric-space.md) $(X,d)$, the [distance to a set](../../../../../distance-to-a-set.md) satisfies

$$
|d(x,F)-d(z,F)|\leq d(x,z).
$$

Indeed, the [triangle inequality](../../../../../triangle-inequality.md) gives $d(x,F)\leq d(x,z)+d(z,F)$, and swapping $x,z$ proves the bound. Thus the two [distance to a set](../../../../../distance-to-a-set.md) functions below are [continuous](../../../../../continuous-function.md). Set

$$
U=\{x:d(x,B)<d(x,C)\},\qquad V=\{x:d(x,C)<d(x,B)\}.
$$

These are disjoint [open sets](../../../../../open-set.md). For $b\in B$, we have $d(b,B)=0$ and $d(b,C)>0$, since $C$ is [closed](../../../../../closed-set.md) and $b\notin C$. Hence $B\subseteq U$. Similarly $C\subseteq V$. Therefore $A\subseteq U\cup V$ and both $U$ and $V$ meet $A$, as required. The construction is a concrete instance of the [normality of every metric space](../../../../../normality-of-every-metric-space.md).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
