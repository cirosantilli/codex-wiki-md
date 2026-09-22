<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An abstract [simplicial complex](../../../../../simplicial-complex.md) consists of a [set](../../../../../set-split.md) $V$ of [vertices of a simplicial complex](../../../../../vertex-of-a-simplicial-complex.md) and a family $K$ of finite nonempty [subsets](../../../../../subset.md) of $V$, called abstract [simplexes](../../../../../simplex.md), such that every [singleton](../../../../../singleton-mathematics.md) $\{v\}$ belongs to $K$ and every nonempty [subset](../../../../../subset.md) of a member of $K$ also belongs to $K$. One may include the [empty set](../../../../../empty-set.md) as an additional face by convention. A member with $k+1$ vertices is a $k$-[simplex](../../../../../simplex.md); its nonempty [subsets](../../../../../subset.md) are its [faces of a simplex](../../../../../face-of-a-simplex.md).

The [geometric realization](../../../../../geometric-realization-of-a-simplicial-complex.md) has the following explicit description using a [barycentric coordinate system](../../../../../barycentric-coordinate-system.md):

$$
|K|=\left\{t:V\to[0,1]:\operatorname{supp}(t)\text{ is finite},\ \sum_{v\in V}t(v)=1,\ \operatorname{supp}(t)\in K\right\}.
$$

Here the [support](../../../../../support.md) is $\operatorname{supp}(t)=\{v:t(v)>0\}$. Each $\rho\in K$ gives a standard geometric [simplex](../../../../../simplex.md)

$$
|\rho|=\{t\in|K|:t(v)=0\text{ for }v\notin\rho\},
$$

with its usual [Euclidean topology](../../../../../euclidean-topology.md). Common [faces of a simplex](../../../../../face-of-a-simplex.md) are identified using the same [barycentric coordinate system](../../../../../barycentric-coordinate-system.md).

Precisely, the [topology](../../../../../topology-split.md) on $|K|$ is defined by declaring $A\subseteq|K|$ [closed](../../../../../closed-set.md) if and only if $A\cap|\rho|$ is [closed](../../../../../closed-set.md) in $|\rho|$ for every $\rho\in K$. Equivalently, use the [quotient topology](../../../../../quotient-topology.md) on the [disjoint union](../../../../../disjoint-union.md) of all the standard geometric [simplexes](../../../../../simplex.md), identifying identical points of common [faces of a simplex](../../../../../face-of-a-simplex.md). For a finite [simplicial complex](../../../../../simplicial-complex.md), this agrees with the [subspace topology](../../../../../subspace-topology.md) in $\mathbb R^V$. For an infinite [simplicial complex](../../../../../simplicial-complex.md), the stated rule specifies the realization [topology](../../../../../topology-split.md) without presuming a finite-dimensional ambient space.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
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
