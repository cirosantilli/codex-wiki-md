<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work near the identity $O$ of a generalized [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md). On the projective chart where $Y\ne0$, use the [local parameter](../../../../../../local-parameter-on-a-smooth-algebraic-curve.md) $t=-x/y$ and the auxiliary coordinate $w=-1/y$. Substitution gives

$$
w=t^3+a_1tw+a_2t^2w+a_3w^2+a_4tw^2+a_6w^3.
$$

The coefficient of $w$ in the linearized equation at $(0,0)$ is one. Consequently, successive coefficient comparison determines a unique [formal power series](../../../../../../formal-power-series.md) $w(t)$, without dividing by any coefficient of the equation. Its initial terms are

$$
w(t)=t^3+a_1t^4+(a_1^2+a_2)t^5+(a_1^3+2a_1a_2+a_3)t^6+O(t^7).
$$

Recover the affine coordinates as Laurent series $x=t/w(t)$ and $y=-1/w(t)$; in particular $x=t^{-2}+O(t^{-1})$ and $y=-t^{-3}+O(t^{-2})$.

The [elliptic curve group law](../../../../../../elliptic-curve-group-law-from-riemann-roch.md) is a regular morphism near $(O,O)$. Applying the local parameter to the sum and passing to completed local rings produces

$$
F(T_1,T_2)=t(P+Q)\in k[[T_1,T_2]].
$$

One can construct the series without any nonunit division. Put

$$
\lambda=\frac{w(T_2)-w(T_1)}{T_2-T_1},\qquad \nu=w(T_1)-\lambda T_1.
$$

The divided difference is an integral [formal power series](../../../../../../formal-power-series.md), including its [tangent line](../../../../../../tangent-line.md) specialization at $T_1=T_2$. The line $w=\lambda t+\nu$ meets the cubic in the two chosen points and a third point $R$. Substitution in the equation shows that its cubic and quadratic coefficients in $t$ are $-A,-B$, where

$$
A=1+a_2\lambda+a_4\lambda^2+a_6\lambda^3,\qquad
B=a_1\lambda+a_2\nu+a_3\lambda^2+2a_4\lambda\nu+3a_6\lambda^2\nu.
$$

Since $\lambda$ has total degree at least two and $\nu$ at least three, $A$ is a unit. The sum of the roots therefore gives

$$
t_R=-T_1-T_2-B/A,\qquad w_R=\lambda t_R+\nu,\qquad
F(T_1,T_2)=-\frac{t_R}{1-a_1t_R-a_3w_R}.
$$

The last expression reflects the third intersection according to the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md). Both denominators have constant term one. This proves integrality of the universal construction and also provides an explicit coefficient algorithm. Expanding it, the resulting [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) begins

$$
\boxed{F(T_1,T_2)=T_1+T_2-a_1T_1T_2-a_2(T_1^2T_2+T_1T_2^2)+O((T_1,T_2)^4).}
$$

The integral coefficient recursion and the unit-denominator addition calculation work universally over $\mathbb Z[a_1,a_2,a_3,a_4,a_6]$; thus these coefficients specialize in every [characteristic of a field](../../../../../../characteristic-of-a-field.md). This is the [initial coefficients of the elliptic formal group at infinity](../../../../../../initial-coefficients-of-the-elliptic-formal-group-at-infinity.md) construction, rather than a definition requiring division by the [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md).

The identity, commutativity and associativity of the [elliptic curve group law](../../../../../../elliptic-curve-group-law-from-riemann-roch.md) give the defining identities of a one-dimensional commutative [formal group law](../../../../../../formal-group-law.md):

$$
F(T,0)=T,\qquad F(X,Y)=F(Y,X),\qquad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

Reflection in the generalized [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) gives its [formal inverse](../../../../../../formal-inverse.md) explicitly:

$$
\iota(T)=-\frac{T}{1-a_1T-a_3w(T)}.
$$

Successive addition gives the multiplication series $[n]_F(T)=nT+O(T^2)$.

In [characteristic zero](../../../../../../characteristic-zero.md), an especially useful description comes from the [invariant differential on an elliptic curve](../../../../../../invariant-differential-on-an-elliptic-curve.md):

$$
\omega=\frac{dx}{2y+a_1x+a_3}=\bigl(1+a_1t+(a_1^2+a_2)t^2+O(t^3)\bigr)\,dt.
$$

Integrating with zero constant term constructs the [formal logarithm](../../../../../../formal-logarithm.md)

$$
L(t)=t+\frac{a_1}{2}t^2+\frac{a_1^2+a_2}{3}t^3+O(t^4).
$$

Translation invariance of the [invariant differential on an elliptic curve](../../../../../../invariant-differential-on-an-elliptic-curve.md) implies $L(F(X,Y))=L(X)+L(Y)$. Thus the [formal logarithm](../../../../../../formal-logarithm.md) converts the [formal group law](../../../../../../formal-group-law.md) into the [formal additive group](../../../../../../formal-additive-group.md) in characteristic zero. Expanding this identity to degree three also recovers the displayed coefficients of $F$; in positive characteristic the integral addition construction remains valid although the logarithmic denominators may not exist.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
