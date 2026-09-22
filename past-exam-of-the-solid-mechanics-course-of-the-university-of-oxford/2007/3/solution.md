<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [hyperelastic material](../../../hyperelastic-material.md) $T_R(F)=DW(F)$. [Material frame indifference](../../../material-frame-indifference.md) of this first Piola-Kirchhoff law means

$$
\boxed{T_R(QF)=Q\,T_R(F)\quad(Q\in SO(3)).}
$$

The spatial [force](../../../force-split.md) components rotate under a superposed rigid [rotation](../../../rotation-mathematics.md), whereas the reference [normal](../../../normal-distribution.md) does not.

If $W(QF)=W(F)$, differentiate with respect to $F$ in direction $H$ to obtain $DW(QF):(QH)=DW(F):H$, hence the displayed [stress](../../../stress.md) transformation. Conversely, assume that [stress](../../../stress.md) transformation. For fixed $Q$, the [derivative](../../../derivative.md) of $W(QF)-W(F)$ with respect to $F$ vanishes. The positive-determinant [matrix](../../../matrix.md) domain is [connected](../../../connected-space.md), as follows from [polar decomposition](../../../polar-decomposition.md) and the [connectedness](../../../connected-space.md) of $SO(3)$ and of the [positive-definite](../../../positive-definite-bilinear-form.md) [cone](../../../cone-geometry.md). Thus $W(QF)-W(F)=c(Q)$, independent of $F$. Iterating gives

$$
W(Q^nF)=W(F)+n c(Q)\qquad(n\in\mathbb Z).
$$

The assumed lower bound on $W$ forces $c(Q)=0$: either nonzero sign would tend to minus infinity for one direction of integer $n$. This proves the required equivalence and explains the use of the lower-bound hypothesis.

In the frame-indifferent setting, [isotropy](../../../isotropy.md) means invariance under reference [rotations](../../../rotation-mathematics.md) as well: $W(FQ)=W(F)$ for $Q\in SO(3)$. The distinction matters: left [rotations](../../../rotation-mathematics.md) encode changes of observer, and right [rotations](../../../rotation-mathematics.md) encode material symmetry.

An orientation-preserving [singular value decomposition](../../../singular-value-decomposition.md) is $F=R\operatorname{diag}(v_1,v_2,v_3)S$, with $R,S\in SO(3)$ and $v_i>0$. [Material frame indifference](../../../material-frame-indifference.md) and [isotropy](../../../isotropy.md) remove $R,S$, leaving a function $\Phi$ of the stretches. Permuting the stretches using signed permutation [rotations](../../../rotation-mathematics.md) does not change the value, so $\Phi$ is [symmetric](../../../symmetric-relation.md). Conversely a [symmetric](../../../symmetric-relation.md) stretch function is unchanged by both left and right [rotations](../../../rotation-mathematics.md), in particular is [isotropic](../../../isotropy.md).

The [eigenvalues](../../../eigenvalue.md) of $B=FF^T$ are $v_i^2$. Its three principal invariants are

$$
I=\operatorname{tr}B=\sum_iv_i^2,\quad
II=\tfrac12[(\operatorname{tr}B)^2-\operatorname{tr}(B^2)]
=\sum_{i<j}v_i^2v_j^2,\quad III=\det B=\prod_iv_i^2.
$$

They determine the unordered positive [eigenvalues](../../../eigenvalue.md) as the roots of $\lambda^3-I\lambda^2+II\lambda-III=0$. Therefore a [symmetric](../../../symmetric-relation.md) stretch function defines a well-defined $h(I,II,III)$ on the admissible invariant triples. Conversely a function of these invariants is a [symmetric](../../../symmetric-relation.md) stretch function, proving the equivalence of all three descriptions.

The printed domain of $\Phi$ must be $(0,\infty)^3$, since it takes three arguments. Also [isotropy](../../../isotropy.md) alone as right invariance would not imply the spectral representation without [material frame indifference](../../../material-frame-indifference.md): $\operatorname{tr}(A FF^T)$ for a fixed nonscalar [symmetric](../../../symmetric-relation.md) [positive-definite](../../../positive-definite-bilinear-form.md) $A$ is right invariant but not generally objective. The equivalence here uses the frame-indifferent constitutive setting.

For the specific energy, [Newton identities](../../../newton-s-identities.md) for the three [eigenvalues](../../../eigenvalue.md) gives $\sum_i v_i^6=I^3-3I\,II+3III$, while $v_1v_2v_3=J=\sqrt{III}$. Thus

$$
\boxed{W=\alpha I+\beta(I^3-3I\,II+3III)+\gamma III^{-1/2}.}
$$

To differentiate it, use

$$
D_FI=2F,\qquad D_FII=2(IF-BF),\qquad
D_FIII=2J\operatorname{cof}F.
$$

These follow from $I=|F|^2$, the displayed [trace](../../../matrix-trace.md) formula for $II$, and $III=J^2$. The three partial derivatives of $h$ are $h_I=\alpha+3\beta I^2-3\beta II$, $h_{II}=-3\beta I$ and $h_{III}=3\beta-\gamma III^{-3/2}/2$. The [chain rule](../../../chain-rule.md) therefore gives

$$
T_R=(2\alpha-6\beta II)F+6\beta I\,BF
+(6\beta J-\gamma J^{-2})\operatorname{cof}F.
$$

Finally $-6\beta II=-3\beta(\operatorname{tr}B)^2+3\beta\operatorname{tr}(B^2)$, and $BF=FF^TF$. This is precisely the requested expression, with the coefficient of $F$ separated from the $BF$ and [cofactor](../../../cofactor.md) terms. The positive sign of the $6\beta J$ term comes from the $3\beta III$ contribution in the energy.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2007](../../2007-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
