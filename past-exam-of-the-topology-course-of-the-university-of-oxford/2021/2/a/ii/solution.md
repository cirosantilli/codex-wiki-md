<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Let $q_S:S^2\to S^2/{\sim_S}$ and $q_D:D^2\to D^2/{\sim_D}$ be the [quotient maps](../../../../../quotient-map.md). The [continuous map](../../../../../continuous-map.md)

$$
h:D^2\longrightarrow S^2,\qquad h(x,y)=\left(x,y,\sqrt{1-x^2-y^2}\right)
$$

is a [homeomorphism](../../../../../homeomorphism.md) onto the upper [hemisphere](../../../../../hemisphere.md); its [inverse function](../../../../../inverse-function.md) is the [restriction](../../../../../restriction-mathematics.md) of the [projection map](../../../../../projection-map.md) $(x,y,z)\mapsto(x,y)$. Every [antipodal pair](../../../../../antipodal-pair.md) on $S^2$ meets that [hemisphere](../../../../../hemisphere.md). Moreover, two points of this [hemisphere](../../../../../hemisphere.md) are antipodal only if both lie on the [equator](../../../../../equator.md). Thus

$$
q_S(h(u))=q_S(h(v))\quad\Longleftrightarrow\quad u\sim_D v.
$$

By the [universal property of the quotient topology](../../../../../universal-property-of-the-quotient-topology.md), $q_S\circ h$ induces a [continuous bijection](../../../../../continuous-bijection.md)

$$
H:D^2/{\sim_D}\longrightarrow S^2/{\sim_S},\qquad H(q_D(u))=q_S(h(u)).
$$

To justify [continuity](../../../../../continuous-function.md) of the [inverse function](../../../../../inverse-function.md), the source is [compact](../../../../../compact-space.md), being a [continuous image of a compact space](../../../../../continuous-image-of-a-compact-space.md) $D^2$; the [Heine-Borel theorem](../../../../../heine-borel-theorem.md) gives [compactness](../../../../../compact-space.md) of $D^2$. The target is [Hausdorff](../../../../../hausdorff-space.md), as follows. For distinct [equivalence classes](../../../../../equivalence-class.md) $[u]\neq[v]$, put

$$
\delta=\min(\|u-v\|,\|u+v\|)>0.
$$

In $S^2$, take the [union](../../../../../set-union.md) $U$ of the two relative [open balls](../../../../../open-ball.md) of radius $\delta/3$ about $u,-u$, and similarly take $V$ about $v,-v$. Every distance between their respective centres is at least $\delta$, so the [triangle inequality](../../../../../triangle-inequality.md) gives $U\cap V=\varnothing$. These [open sets](../../../../../open-set.md) contain entire [antipodal pairs](../../../../../antipodal-pair.md), hence $q_S^{-1}(q_S(U))=U$ and similarly for $V$. The [quotient topology](../../../../../quotient-topology.md) therefore makes $q_S(U)$ and $q_S(V)$ disjoint [open](../../../../../open-set.md) [neighbourhoods](../../../../../neighbourhood-mathematics.md) of the two classes.

The [compact-to-Hausdorff continuous bijection theorem](../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) now gives **the required [homeomorphism](../../../../../homeomorphism.md) $H$**.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
