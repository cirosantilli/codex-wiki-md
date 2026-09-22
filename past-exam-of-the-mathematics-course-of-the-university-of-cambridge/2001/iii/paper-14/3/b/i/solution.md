<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use coordinates in which $l=\{x_2=x_3=0\}$ and write the defining cubic as

$$
F=x_2Q_2+x_3Q_3
$$

with [homogeneous polynomials](../../../../../../../homogeneous-polynomial.md) $Q_2,Q_3$ of degree two. Their restrictions $A=Q_2|_l$, $B=Q_3|_l$ have no common zero: at such a zero all first partial derivatives of $F$ would vanish. The rational projection $[x_2:x_3]$ therefore extends to a [morphism of algebraic varieties](../../../../../../../morphism-of-algebraic-varieties.md)

$$
f:S\longrightarrow\mathbb P^1,
\qquad f|_l=[-B:A].
$$

Indeed, wherever $Q_2\ne0$, the surface equation gives $[x_2:x_3]=[-Q_3:Q_2]$, which remains regular on $l$; the analogous formula works wherever $Q_3\ne0$.

For the plane with $x_2=sw$, $x_3=tw$, its [plane section](../../../../../../../plane-section.md) is $l$ together with the residual [plane conic](../../../../../../../plane-conic.md)

$$
q_{s,t}(u,v,w)=sQ_2(u,v,sw,tw)+tQ_3(u,v,sw,tw)=0.
$$

These residual [plane conics](../../../../../../../plane-conic.md) are exactly the [fibres of a morphism](../../../../../../../fiber-of-a-morphism.md) of $f$, giving the [conic bundle from a line on a smooth cubic surface](../../../../../../../conic-bundle-from-a-line-on-a-smooth-cubic-surface.md). The family itself is smooth: off $l$ it is the graph of projection, and over $l$ the condition $sA+tB=0$ chooses the unique value $[-B:A]$.

Write $q_{s,t}=z^{\mathsf T}M(s,t)z$ with $z=(u,v,w)^{\mathsf T}$ and $M$ symmetric. The degrees of its entries in $(s,t)$ are

$$
\begin{pmatrix}1&1&2\\1&1&2\\2&2&3\end{pmatrix}.
$$

Thus the [conic discriminant](../../../../../../../conic-discriminant.md) $\Delta(s,t)=\det M(s,t)$ is a [homogeneous polynomial](../../../../../../../homogeneous-polynomial.md) of degree five.

Smoothness also shows that every zero of $\Delta$ is simple and has [matrix rank](../../../../../../../matrix-rank.md) two. To see the first point, at a rank-two singular fibre let $z_0$ span the kernel and use a local base coordinate $\tau$. All fibre-coordinate derivatives vanish at $z_0$, so smoothness of the total family requires $z_0^{\mathsf T}M'(\tau)z_0\ne0$. Since the [adjugate matrix](../../../../../../../adjugate-matrix.md) of a rank-two symmetric matrix is a nonzero scalar multiple of $z_0z_0^{\mathsf T}$, the determinant derivative is nonzero. If the rank were at most one, the projective kernel would contain a line, on which the quadratic $z^{\mathsf T}M'z$ has a zero over the [algebraically closed field](../../../../../../../algebraically-closed-field.md); that point would be singular in the total family. This proves the [reduced singular fibres of a smooth conic bundle](../../../../../../../reduced-singular-fibres-of-a-smooth-conic-bundle.md) assertion and also rules out $\Delta$ vanishing identically.

The [discriminant quintic of a cubic surface conic bundle](../../../../../../../discriminant-quintic-of-a-cubic-surface-conic-bundle.md) consequently has five distinct zeros in $\mathbb P^1$. At each, a rank-two [plane conic](../../../../../../../plane-conic.md) splits into two distinct [projective lines](../../../../../../../projective-line.md) $l_i,l_i'$. Neither equals $l$: that would require $sA+tB$ to vanish identically, making $A,B$ proportional, contrary to their having no common zero. The original [plane section](../../../../../../../plane-section.md) is therefore $l\cup l_i\cup l_i'$, proving the required coplanarity and giving **five distinct pairs**.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 14](../../../../paper-14-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
