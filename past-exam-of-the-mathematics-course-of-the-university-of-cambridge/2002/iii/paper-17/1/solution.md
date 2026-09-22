<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [finite CW complex](../../../../../finite-cw-complex.md) can be defined without assuming separation properties in advance. Start with a finite discrete set $X^0$. Inductively form $X^k$ from $X^{k-1}\sqcup\coprod_\alpha D^k_\alpha$ by identifying each boundary point with its image under a continuous attaching map $a_\alpha:S^{k-1}\to X^{k-1}$. Only finitely many disks are attached in total, and $X=X^N$ for some finite $N$. The interiors of the disks are its cells. Its [weak topology of a CW complex](../../../../../weak-topology-of-a-cw-complex.md) is the final topology of the characteristic maps: a subset is closed exactly when its inverse image in every characteristic disk is closed. In this finite construction it is the topology obtained by the successive quotients. Closure-finiteness is automatic because there are only finitely many cells.

Here is a direct proof of both requested topological properties, without presupposing that arbitrary attaching maps give a triangulable space. Suppose the [compact](../../../../../compact-space.md) previous stage $Y$ embeds by $e:Y\hookrightarrow\mathbb R^m$, and attach one $k$-cell, $k\ge1$. Extend the boundary coordinate map radially by

$$
G(ru)=r\,e(a(u)),\quad u\in S^{k-1},\qquad G(0)=0.
$$

It is continuous at zero because the image of the [sphere](../../../../../sphere.md) is bounded. Map the two pieces into $\mathbb R^{m+k+1}$ by

$$
y\longmapsto(e(y),0,0),\qquad x\longmapsto\bigl(G(x),(1-|x|)x,1-|x|\bigr).
$$

At $|x|=1$ these agree with the attaching identification. They therefore induce a [continuous map](../../../../../continuous-map.md) on the quotient. Its restriction to the old stage is injective. An interior point has positive last coordinate $t=1-|x|$, and the preceding coordinate block recovers $x$ by division by $t$. Hence it cannot coincide with an old point or another interior point. The induced map is injective.

The quotient is [compact](../../../../../compact-space.md), being the image of a [compact](../../../../../compact-space.md) [disjoint union](../../../../../disjoint-union.md). A continuous injection into [Euclidean space](../../../../../euclidean-norm.md) is [Hausdorff](../../../../../hausdorff-space.md), by inverse images of disjoint separating neighborhoods; it is also a [homeomorphism](../../../../../homeomorphism.md) onto its image because closed subsets of the [compact](../../../../../compact-space.md) source have [compact](../../../../../compact-space.md), hence closed, images in the [Hausdorff](../../../../../hausdorff-space.md) target. Finite discrete $X^0$ embeds in $\mathbb R$, and induction over the finite list of cells proves **$X$ is [Hausdorff](../../../../../hausdorff-space.md) and its weak topology is exactly an induced Euclidean [subspace topology](../../../../../subspace-topology.md)**. This is [Euclidean embedding by finite cell attachment](../../../../../euclidean-embedding-by-finite-cell-attachment.md); no optimal ambient dimension is needed.

For [Real projective space](../../../../../real-projective-space.md), filter by $\mathbb{RP}^0\subset\cdots\subset\mathbb{RP}^n$. The complement of $\mathbb{RP}^{k-1}$ in $\mathbb{RP}^k$ is an affine $k$-cell. A characteristic disk is a hemisphere of $S^k$, whose boundary is attached by the antipodal quotient $S^{k-1}\to\mathbb{RP}^{k-1}$. Thus there is one cell in every dimension $0,\ldots,n$.

The incidence number is the sum of the two sheet contributions. Fixing the orientation of one sheet gives degree one; the other differs by the antipodal map on $S^{k-1}$, whose degree is $(-1)^k$. Consequently the [cellular homology of real projective space](../../../../../cellular-homology-of-real-projective-space.md) has

$$
C_k=\mathbb Z\quad(0\le k\le n),\qquad d_k=1+(-1)^k=\begin{cases}2&k\text{ even},\\0&k\text{ odd}.\end{cases}
$$

Taking kernels modulo images gives, for $n\ge1$,

$$
\boxed{H_q(\mathbb{RP}^n;\mathbb Z)=\begin{cases}\mathbb Z&q=0,\\\mathbb Z/2&0<q<n\text{ and }q\text{ odd},\\\mathbb Z&q=n\text{ and }n\text{ odd},\\0&\text{otherwise}.\end{cases}}
$$

Over $\mathbb R$, multiplication by two is invertible, so

$$
\boxed{H_q(\mathbb{RP}^n;\mathbb R)=\begin{cases}\mathbb R&q=0,\text{ or }q=n\text{ with }n\text{ odd},\\0&\text{otherwise}.\end{cases}}
$$

Over $\mathbb F_2=\mathbb Z/2$, every differential vanishes, giving **$H_q(\mathbb{RP}^n;\mathbb F_2)=\mathbb F_2$ for $0\le q\le n$, and zero otherwise**. For $n=0$ the space is a point and only degree-zero [homology](../../../../../homology-split.md) is present, with the chosen coefficient [group](../../../../../group-split.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
