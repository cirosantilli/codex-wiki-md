<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

To establish [strong NP-completeness](../../../../../strong-np-completeness.md), use an explicit [adjacency matrix](../../../../../adjacency-matrix.md) encoding for a finite [simple graph](../../../../../simple-graph.md), with enough length information to recover its number $N$ of [vertices](../../../../../vertex-graph-theory.md). Let $\operatorname{bin}(k)$ be the canonical [binary numeral system](../../../../../binary-numeral-system.md) representation of the nonnegative [integer](../../../../../integer-split.md) $k$. Define

$$
\mathcal L_{\mathrm{Clique}}
=\{\langle\operatorname{enc}(G),\operatorname{bin}(k)\rangle:
G\text{ has a clique of size }k\},
$$

and, using the [unary numeral system](../../../../../unary-numeral-system.md) for $k$,

$$
\mathcal L_{u\mathrm{Clique}}
=\{\langle\operatorname{enc}(G),1^k\rangle:
G\text{ has a clique of size }k\}.
$$

The surrounding pairing syntax delimits the two components, so the empty unary field can encode $k=0$ if zero is included in the convention for [natural numbers](../../../../../natural-number.md). Malformed descriptions are excluded from both [formal languages](../../../../../formal-language.md).

Fix a unary no-instance $u_0$, for example one isolated [vertex](../../../../../vertex-graph-theory.md) with requested size $2$. The [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) is

$$
f(\langle\operatorname{enc}(G),\operatorname{bin}(k)\rangle)
=\begin{cases}
\langle\operatorname{enc}(G),1^k\rangle,&0\leq k\leq N,\\
u_0,&k>N.
\end{cases}
$$

Map malformed [inputs](../../../../../input-computer-science.md) to $u_0$ too. When $k\leq N$, only the numerical representation changes, so the existence of a $k$-[clique](../../../../../clique-graph-theory.md) is unchanged. When $k>N$, the original instance is false, since a [subset](../../../../../subset.md) of [vertices](../../../../../vertex-graph-theory.md) cannot be larger than the whole [vertex set](../../../../../vertex-set.md); $u_0$ is false as required.

The important size bound is $k\leq N$ in the branch that writes $1^k$. The original explicit [graph](../../../../../graph-split.md) description already has length at least $N$, so the output has [polynomial](../../../../../polynomial-split.md) length and can be written in [polynomial time](../../../../../polynomial-time.md). If a huge [binary numeral system](../../../../../binary-numeral-system.md) value $k$ is supplied, compare it with $N$ using its digit length and, when needed, a digit comparison; do not first allocate or print $k$ symbols. Merely replacing an unrestricted binary $k$ by $1^k$ would not be a valid [polynomial-time reduction](../../../../../polynomial-time-reduction.md).

Thus $\mathcal L_{\mathrm{Clique}}\leq_p\mathcal L_{u\mathrm{Clique}}$. The unary version is in [NP](../../../../../np-complexity.md) by the same [clique](../../../../../clique-graph-theory.md) [complexity certificate](../../../../../certificate-complexity.md) verification, and is [NP-hard](../../../../../np-hardness.md) by this [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) and part (e). Therefore

$$
\boxed{\mathrm{Clique}\text{ is strongly NP-complete}.}
$$

This conclusion uses the conventional explicit [graph](../../../../../graph-split.md) encoding; a succinct circuit description of a [graph](../../../../../graph-split.md) would be a different [input](../../../../../input-computer-science.md) representation and a different problem.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
