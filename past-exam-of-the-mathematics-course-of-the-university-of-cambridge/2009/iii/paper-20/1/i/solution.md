<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $x,y$ be the generators associated with the two pairs of [one-handle](../../../../../../one-handle.md) feet. Following the attaching circle across the identifications marked $a,b$ and $c,d$ gives the word $xyx^{-1}y^{-1}$, up to reversal and changing generator orientations. Thus the [van Kampen theorem](../../../../../../seifert-van-kampen-theorem.md) gives

$$
\boxed{\pi_1(W)=\langle x,y\mid xyx^{-1}y^{-1}=1\rangle\cong\mathbb Z^2.}
$$

The [handle decomposition](../../../../../../handle-decomposition.md) has cellular groups $C_0=\mathbb Z$, $C_1=\mathbb Z^2$, $C_2=\mathbb Z$, with no higher groups. The boundary of the two-cell is the abelianized attaching word, which is zero. Hence

$$
\boxed{H_j(W;\mathbb Z)=\begin{cases}\mathbb Z,&j=0,2,\\\mathbb Z^2,&j=1,\\0,&j\ge3.\end{cases}}
$$

The zero framing is the product framing of the [commutator handlebody of the torus](../../../../../../commutator-handlebody-of-the-torus.md), so the represented manifold is $T^2\times D^2$ and its [intersection form](../../../../../../intersection-form.md) is $(0)$. In particular its boundary is $T^2\times S^1=T^3$.

The boundary [homology](../../../../../../homology-split.md) can also be obtained without using the product identification. By [Poincare-Lefschetz duality](../../../../../../lefschetz-duality.md), $H_3(W,\partial W)=H^1(W)=\mathbb Z^2$ and $H_2(W,\partial W)=H^2(W)=\mathbb Z$. The map $H_2(W)\to H_2(W,\partial W)$ is its zero [intersection form](../../../../../../intersection-form.md). The [long exact sequence of a pair](../../../../../../long-exact-sequence-in-relative-homology.md) then gives split sequences

$$
0\to\mathbb Z^2\to H_2(\partial W)\to\mathbb Z\to0,\qquad
0\to\mathbb Z\to H_1(\partial W)\to\mathbb Z^2\to0.
$$

The boundary is connected and oriented, so its zeroth and third [homology](../../../../../../homology-split.md) are both $\mathbb Z$. Therefore

$$
\boxed{H_j(\partial W;\mathbb Z)=\begin{cases}\mathbb Z,&j=0,3,\\\mathbb Z^3,&j=1,2,\\0,&j\ge4.\end{cases}}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
