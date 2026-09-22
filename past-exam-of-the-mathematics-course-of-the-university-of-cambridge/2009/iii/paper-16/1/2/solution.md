<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $a$ be the projective-line loop and $b$ the core loop of the [Möbius band](../../../../../../mobius-band.md). The boundary of the [Möbius band](../../../../../../mobius-band.md) goes twice around its core. Its boundary inclusion is a [cofibration](../../../../../../cofibration.md), so replacing the gluing map by a homotopic cellular degree-$n$ map preserves the homotopy type. More precisely, the band is a [mapping cylinder](../../../../../../mapping-cylinder.md) of the boundary double covering onto the core circle. After attaching its other end and collapsing the connecting tree, the resulting space has a homotopy-equivalent [CW complex](../../../../../../cw-complex.md) with one vertex, edges $a,b$, and two two-cells with attaching words

$$
a^2,\qquad a^{-n}b^2.
$$

The first is the projective-plane face; the second records equality of the attached boundary loop $a^n$ and the band boundary loop $b^2$. Taking exponent sums gives the [cellular chain complex](../../../../../../cellular-chain-complex.md)

$$
0\longrightarrow\mathbb Z^2\xrightarrow{\;D\;}\mathbb Z^2\xrightarrow{\;0\;}\mathbb Z\longrightarrow0,\qquad
D=\begin{pmatrix}2&-n\\0&2\end{pmatrix}.
$$

Since $\det D=4$, its kernel is zero. The first invariant factor in the [Smith normal form](../../../../../../smith-normal-form.md) is the greatest common divisor of its entries, $d=\gcd(2,n)$, and the second is $4/d$. Hence

$$
\boxed{H_0(X;\mathbb Z)=\mathbb Z,\qquad H_1(X;\mathbb Z)=\begin{cases}\mathbb Z/4,&n\text{ odd},\\(\mathbb Z/2)^2,&n\text{ even},\end{cases}\qquad H_j(X;\mathbb Z)=0\ (j\geq2).}
$$

This includes $n=0$ and negative degrees. The [fundamental group after attaching a Möbius band](../../../../../../fundamental-group-after-attaching-a-mobius-band.md) is $\langle a,b\mid a^2=1,\ b^2=a^n\rangle$, consistent with the computed abelianization. The calculation is an example of [homology after attaching a Möbius band to the real projective plane](../../../../../../homology-after-attaching-a-mobius-band-to-the-real-projective-plane.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
