<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $\tau$ to be the [ordinary topology on infinite subsets](../../../../../../ordinary-topology-on-infinite-subsets.md), whose basic cylinders $[s]$ fix a finite [initial segment](../../../../../../initial-segment.md). Let

$$
D=\{Z\in[\mathbb N]^\omega:\mathbb N\setminus Z\text{ is finite}\}.
$$

This is a [dense countable family of cofinite infinite subsets](../../../../../../dense-countable-family-of-cofinite-infinite-subsets.md). It is countable because finite complements form a countable family. Each singleton is $\tau$-[closed](../../../../../../closed-set.md): distinct increasing enumerations differ at some finite coordinate, which separates them by cylinders. No singleton has [interior](../../../../../../interior-topology.md), since every cylinder admits more than one infinite continuation. Thus every singleton is $\tau$-[nowhere dense](../../../../../../nowhere-dense-set.md), and $D$ is $\tau$-[meagre](../../../../../../meagre-set.md).

On the other hand, every cylinder $[s]$ contains the [cofinite set](../../../../../../cofinite-set.md) $s\cup\{n:n>\max s\}$, with $\max\varnothing=0$. Hence $D$ is $\tau$-[dense](../../../../../../dense-set.md), its [closure](../../../../../../closure-topology.md) is all of $X$, and

$$
\boxed{D\text{ is }\tau\text{-meagre but not }\tau\text{-nowhere dense}.}
$$

The paper does not define its symbol $\tau$. If the course instead uses it for the [Ramsey cone topology](../../../../../../ramsey-cone-topology.md), with basic neighborhoods $[A]^\omega$ and no finite stem, use $X$ itself as the example. For $D_j=\{Z:\min Z=j\}$, its cone-[closure](../../../../../../closure-topology.md) is $\{Z:j\in Z\}$: every cone neighborhood of a set containing $j$ contains an infinite subset of minimum $j$, while a cone based on a set omitting $j$ misses $D_j$. This [closure](../../../../../../closure-topology.md) has empty [interior](../../../../../../interior-topology.md), because every infinite reservoir can be thinned to omit $j$. Thus every $D_j$ is cone-[nowhere dense](../../../../../../nowhere-dense-set.md), and $X=\bigcup_{j\geq1}D_j$ is cone-[meagre](../../../../../../meagre-set.md) but is not cone-[nowhere dense](../../../../../../nowhere-dense-set.md). This supplies the requested example under either convention, without conflating the two topologies.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
