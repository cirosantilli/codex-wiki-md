<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an invertible [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md), differentiating $Y_\lambda=AY$ in $z$ and $Y_z=BY$ in $\lambda$ gives $Y_{\lambda z}=(A_z+AB)Y$ and $Y_{z\lambda}=(B_\lambda+BA)Y$. Thus the necessary and sufficient compatibility identity is

$$
\boxed{F:=A_z-B_\lambda+[A,B]=0.}
$$

Here both [derivatives](../../../../../derivative.md) must use the actual deformation variable $z$; the printed $t$ has not been defined. The [isomonodromic deformation](../../../../../isomonodromic-deformation.md) identity can be checked as a [polynomial](../../../../../polynomial-split.md) in $\lambda$, without assuming the conclusion.

First retain the coefficients actually printed in the PDF. Write $p=u'$, $d=w+z/2$, and introduce the two residuals

$$
K=w'-\frac{2u'w}{u},\qquad H=u''+du.
$$

Direct [matrix multiplication](../../../../../matrix-multiplication.md) and differentiation give

$$
\begin{aligned}
F={}&\lambda^2\begin{pmatrix}0&0\\(2-z)w/u&0\end{pmatrix}
+\lambda\begin{pmatrix}(z-2)w/2&0\\
-(w+zw')/u+(z+2)u'w/u^2&-(z-2)w/2\end{pmatrix}\\
&+\begin{pmatrix}K&H\\2wH/u^2+2u'K/u^2&-K\end{pmatrix}.
\end{aligned}
$$

For example, the quadratic lower entry is the difference between $[D,B_0]_{21}=2w/u$ and the contribution $(A_1)_{21}=-zw/u$; it does not cancel. The constant lower entry follows by differentiating $2u'w/u^2$ and collecting it as $2wH/u^2+2u'K/u^2$. These entries also provide independent checks of the two most important cancellations.

Work on an open connected deformation domain where $u\ne0$, as the [matrices](../../../../../matrix.md) require. The quadratic entry forces $(2-z)w=0$ throughout the domain, hence $w\equiv0$ by continuity, including a possible point $z=2$. All remaining entries then vanish exactly when $u''+(z/2)u=0$. Thus the literal answer is

$$
\boxed{w\equiv0,\qquad u''+\frac z2u=0.}
$$

This is a rescaled [Airy function](../../../../../airy-function.md) equation: with $\xi=-2^{-1/3}z$, the equation is $u_{\xi\xi}-\xi u=0$, so $u=c_1\operatorname{Ai}(\xi)+c_2\operatorname{Bi}(\xi)$ on a domain avoiding its zeros. In particular, choose the local solution with $u(1)=u'(1)=1$ and $w=0$. It gives compatible [matrices](../../../../../matrix.md) but violates the printed $w=u'$. This proves that the requested assertion is false for the original coefficients, independently of the undefined $t/z$ in the printed [differential equation](../../../../../differential-equation-split.md).

For completeness, use the explicitly corrected lower coefficient $(A_1)_{21}=-2w/u$ from the preceding solution. The same multiplication gives the much simpler residual

$$
F=\lambda\begin{pmatrix}0&0\\-2K/u&0\end{pmatrix}
+\begin{pmatrix}K&H\\2wH/u^2+2u'K/u^2&-K\end{pmatrix}.
$$

Consequently compatibility is equivalent to $K=H=0$. The first equation integrates without dividing by $w$:

$$
\left(\frac{w}{u^2}\right)'=\frac1{u^2}\left(w'-\frac{2u'w}{u}\right)=0.
$$

The [constant of integration](../../../../../constant-of-integration.md) $C$ therefore satisfies $w=Cu^2$, and the second equation becomes

$$
\boxed{w=Cu^2,\qquad u''+Cu^3+\frac z2u=0.}
$$

Conversely these two equations give $K=H=0$, and substitution makes every residual entry vanish, proving sufficiency as well as necessity. This is the [quadratic spectral Lax pair for zero-parameter Painlevé II](../../../../../quadratic-spectral-lax-pair-for-zero-parameter-painleve-ii.md). For $C\ne0$, choose constants $b,a$ with $b^3=-2$ and $Ca^2b^2=-2$, set $z=bx$, $u=aq(x)$, and obtain $q''=2q^3+xq$, the zero-parameter [Painlevé II equation](../../../../../painleve-ii-equation.md). For $C=0$ it reduces to the [Airy function](../../../../../airy-function.md) equation. Even with this correction, the conclusions are $w=Cu^2$ and the coefficient $z/2$, rather than the incompatible expressions printed in the question.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
