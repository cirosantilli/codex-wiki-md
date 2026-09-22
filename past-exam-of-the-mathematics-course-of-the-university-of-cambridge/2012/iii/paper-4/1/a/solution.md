<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a separation $\operatorname{Spec}R=U\sqcup V$ into two nonempty [clopen sets](../../../../../../clopen-set.md). Both are closed in the [Zariski topology](../../../../../../zariski-topology.md), so write $U=V(I)$ and $V=V(J)$ for [ideals](../../../../../../ideal.md) $I,J$. Their disjointness gives $V(I+J)=\varnothing$. A proper [ideal](../../../../../../ideal.md) lies in a [maximal ideal](../../../../../../maximal-ideal.md), so this forces $I+J=R$.

Their union is all of the [spectrum of a commutative ring](../../../../../../spectrum-of-a-commutative-ring.md), and $V(I)\cup V(J)=V(IJ)$. Thus every [prime ideal](../../../../../../prime-ideal.md) contains $IJ$, so

$$
IJ\subseteq\bigcap_{\mathfrak p\in\operatorname{Spec}R}\mathfrak p
=\sqrt{(0)}=0.
$$

The last equality uses that $R$ is a [reduced ring](../../../../../../reduced-ring.md). For [comaximal ideals](../../../../../../comaximal-ideals.md), $I\cap J=IJ$: if $i+j=1$ and $r\in I\cap J$, then $r=ri+rj\in IJ$. Therefore the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives

$$
\boxed{R\cong R/I\times R/J}.
$$

The isomorphism sends $r$ to its two residue classes. Its kernel is $I\cap J=0$; for surjectivity, $a\bmod I$ and $b\bmod J$ are obtained from $aj+bi$, where $i\in I$, $j\in J$ and $i+j=1$. The two factors are nonzero because $U,V$ are nonempty, so $I,J$ are proper.

This is a [disconnected reduced spectrum product decomposition](../../../../../../disconnected-reduced-spectrum-product-decomposition.md). The elements $i,j$ also satisfy $ij=0$, $i^2=i$, $j^2=j$, exhibiting the [ring product decomposition by an idempotent](../../../../../../ring-product-decomposition-by-an-idempotent.md). No Noetherian hypothesis is required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
