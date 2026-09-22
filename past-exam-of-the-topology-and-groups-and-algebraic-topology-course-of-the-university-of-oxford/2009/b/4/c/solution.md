<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a(x)=-x$ be the [antipodal map](../../../../../antipodal-map.md), whose degree is $(-1)^{n+1}$. The invariance condition is $f\circ a=f$. Multiplicativity of degree gives $\deg(f)(-1)^{n+1}=\deg(f)$, so if $n$ is even,

$$
\boxed{\deg(f)=0}.
$$

For odd $n$, factor the invariant map uniquely through the quotient $q:S^n\to\mathbb{RP}^n$, writing $f=gq$. The standard orientability and homology facts for [Real projective space](../../../../../real-projective-space.md) are that $\mathbb{RP}^n$ is orientable in odd dimension and has top integral homology $\mathbb Z$. With compatible [orientation](../../../../../orientation-of-a-simplex.md) the double cover $q$ has degree two: both local sheets preserve [orientation](../../../../../orientation-of-a-simplex.md) because the [antipodal map](../../../../../antipodal-map.md) does. Thus $g_*$ is multiplication by an integer $k$ and $\deg(f)=2k$.

Every such integer occurs. In the oriented projective space, choose a small oriented closed ball and collapse its exterior to a point. The resulting map $c:\mathbb{RP}^n\to S^n$ has degree one, because a point in the interior image has one [orientation](../../../../../orientation-of-a-simplex.md)-preserving preimage. Composing it with a degree-$k$ [sphere](../../../../../sphere.md) map from part (b) gives

$$
f=\alpha_k\circ c\circ q,\qquad\boxed{\deg(f)=2k}.
$$

Here $\alpha_k$ denotes the dimension-$n$ map constructed by suspension. The factorization through $q$ makes the resulting map antipodally invariant.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../../split.md)
6. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
