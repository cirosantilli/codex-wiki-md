# Conformal automorphism of the upper half-plane

↑ **Parent:** [Upper half-plane (complex analysis)](upper-half-plane-complex-analysis.md)

Every [conformal automorphism of the upper half-plane](conformal-automorphism-of-the-upper-half-plane.md) is a [Möbius transformation](mobius-transformation.md) with real coefficients and positive [determinant](determinant.md), and conversely every such map is a [conformal bijection](biholomorphism.md) of the [upper half-plane](upper-half-plane-complex-analysis.md) to itself:

$$
f(z)=\frac{az+b}{cz+d},\qquad a,b,c,d\in\mathbb R,\qquad \Delta=ad-bc>0.
$$

The real-coefficient and sign conditions matter. The complex [Möbius transformation](mobius-transformation.md) $z\mapsto iz$ sends $i$ to $-1$ on the [boundary](boundary-of-a-set.md), while the real [Möbius transformation](mobius-transformation.md) $z\mapsto1/z$ has negative [determinant](determinant.md) and sends $i$ to $-i$ in the [lower half-plane](lower-half-plane.md). [Romik, Complex Analysis, Homework 4, page 3, automorphism statement 5](https://math.ucdavis.edu/~romik/data/uploads/teaching/math205a-2018/mat205a-2018-hw4.pdf)

For two concrete [upper half-plane automorphisms](conformal-automorphism-of-the-upper-half-plane.md), take

$$
T(z)=z+1,\quad A_T=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad S(z)=-\frac1z,\quad A_S=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.
$$

Both [matrices](matrix.md) have [determinant](determinant.md) one. Here $T(i)=1+i$, $S(i)=i$, and $S(1+i)=(-1+i)/2$. On the extended [real line](real-line.md), $T$ fixes infinity and $S$ exchanges zero and infinity. On the [unit disc](unit-disc.md), the same maps become $C\circ T\circ C^{-1}$ and $C\circ S\circ C^{-1}$; the second is simply $w\mapsto-w$.

Multiplying all four coefficients by a nonzero real scalar leaves $f$ unchanged. Dividing them by $\sqrt\Delta$ normalizes the [determinant](determinant.md) to one; the two remaining representatives $A$ and $-A$ give the same map. Thus the [group](group-split.md) under [function composition](function-composition.md) is the [projective special linear group](projective-special-linear-group.md)

$$
\operatorname{Aut}(\mathbb H)\cong PSL_2(\mathbb R)=SL_2(\mathbb R)/\{I,-I\},
$$

where $SL_2(\mathbb R)$ is the [real special linear group of degree two](real-special-linear-group-of-degree-two.md). Composition of the [Möbius transformations](mobius-transformation.md) corresponds to multiplication of their [matrices](matrix.md). [Series, section 1.3, Theorem 1.27](https://warwick.ac.uk/fac/sci/maths/people/staff/caroline_series/hyperbolic_geometry_ma448_lecture_notes.pdf)

On the [boundary](boundary-of-a-set.md),

$$
f'(x)=\frac{\Delta}{(cx+d)^2}>0\qquad(cx+d\ne0).
$$

So $f$ preserves the cyclic [boundary orientation](boundary-orientation.md) of the extended [real line](real-line.md); when $c\ne0$, its [pole](pole.md) at $-d/c$ prevents treating it as a single increasing [function](function-split.md) across that point on the ordinary [real line](real-line.md). Three distinct [boundary](boundary-of-a-set.md) images determine a [Möbius transformation](mobius-transformation.md) uniquely, but an [upper half-plane automorphism](conformal-automorphism-of-the-upper-half-plane.md) can realize only triples with matching cyclic [boundary orientation](boundary-orientation.md).

A brief proof outline starts with the identities

$$
\operatorname{Im}f(z)=\frac{\Delta\operatorname{Im}z}{|cz+d|^2},\qquad f^{-1}(w)=\frac{dw-b}{-cw+a}.
$$

They show that $f$ and its [inverse function](inverse-function.md) preserve the [upper half-plane](upper-half-plane-complex-analysis.md). For completeness of the classification, conjugate an arbitrary [conformal bijection](biholomorphism.md) by the [Cayley transform](cayley-transform-complex-analysis.md). Normalize its image of zero with an [automorphism of the unit disk](automorphism-of-the-unit-disk.md), then apply the [Schwarz lemma](schwarz-lemma.md) to the resulting map and its [inverse function](inverse-function.md); both inequalities force a rotation. Conjugating back gives the real [Möbius transformation](mobius-transformation.md) above.

Finally, $|f'(z)|=\Delta/|cz+d|^2$ and the displayed [imaginary part](imaginary-part.md) identity show that $|df(z)|/\operatorname{Im}f(z)=|dz|/\operatorname{Im}z$. Every [upper half-plane automorphism](conformal-automorphism-of-the-upper-half-plane.md) is therefore also an [isometry](isometry.md) of the [Poincaré half-plane model](poincare-half-plane-model.md). The same formulas describe both [holomorphic](holomorphic-function-split.md) coordinate symmetries and motions of the [hyperbolic plane](hyperbolic-plane.md).

## ↑ Ancestors (6)

1. [Upper half-plane (complex analysis)](upper-half-plane-complex-analysis.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Conformal automorphism of the upper half-plane](conformal-automorphism-of-the-upper-half-plane.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-36/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-203/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-203/4/c/solution.md)
- [Target-change locality of SLE6](target-change-locality-of-sle6.md)
- [Target-dependent continuation of SLE6](target-dependent-continuation-of-sle6.md)
