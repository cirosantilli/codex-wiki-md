<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With determinant-one normalization, the necessary and sufficient condition for [sphere rotations as special-unitary Möbius transformations](../../../../../sphere-rotations-as-special-unitary-mobius-transformations.md) is

$$
\boxed{c=-\overline b,\qquad d=\overline a,\qquad |a|^2+|b|^2=1.}
$$

Equivalently, the matrix $M=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ belongs to the [special unitary group](../../../../../special-unitary-group.md) $SU(2)$. The two determinant-one representatives $M$ and $-M$ induce the same [Möbius transformation](../../../../../mobius-transformation.md), and both satisfy this condition.

Use north-pole [stereographic projection](../../../../../stereographic-projection.md) in the direction from the plane to the [sphere](../../../../../sphere.md):

$$
\varphi(z)=\frac{(2\operatorname{Re}z,2\operatorname{Im}z,|z|^2-1)}{1+|z|^2},\qquad
\varphi(\infty)=(0,0,1).
$$

Its chord-distance identity is $|\varphi(z)-\varphi(w)|=2\chi(z,w)$, where $\chi$ is the [chordal metric](../../../../../chordal-metric.md). Direct subtraction, using $ad-bc=1$, gives

$$
\chi(g(z),g(w))=
\frac{|z-w|}{\sqrt{H(z)H(w)}},\qquad
H(z)=|az+b|^2+|cz+d|^2.
$$

This is first calculated away from [poles](../../../../../pole.md) and then extended continuously to the [Riemann sphere](../../../../../riemann-sphere.md). A [sphere](../../../../../sphere.md) [rotation](../../../../../rotation-mathematics.md) preserves chord distances, so for distinct finite nonpole points

$$
\frac{H(z)}{1+|z|^2}\frac{H(w)}{1+|w|^2}=1.
$$

Using three distinct points shows all these positive ratios equal one. Hence $H(z)=1+|z|^2$ everywhere. Comparing its coefficients gives

$$
|a|^2+|c|^2=1,\quad |b|^2+|d|^2=1,\quad
 a\overline b+c\overline d=0.
$$

Thus $M$ is a [unitary matrix](../../../../../unitary-matrix.md). Comparing $M^{-1}=M^*$ with $M^{-1}=\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$ proves the boxed relations.

Conversely, these relations give $H(z)=1+|z|^2$, so the induced [sphere](../../../../../sphere.md) map $T=\varphi g\varphi^{-1}$ preserves all Euclidean chord distances. Such a [bijection](../../../../../bijection.md) of the unit [sphere](../../../../../sphere.md) is the restriction of an [orthogonal matrix](../../../../../orthogonal-matrix.md): let $v_j=T(e_j)$; preservation of distances makes these an orthonormal basis, and $T(p)\cdot v_j=p\cdot e_j$ forces $T(p)=\sum_jp_jv_j$. Finally the [Möbius transformation](../../../../../mobius-transformation.md) is holomorphic with positive real Jacobian at every ordinary coordinate point. Conjugating by [stereographic projection](../../../../../stereographic-projection.md) preserves orientation, so this [orthogonal matrix](../../../../../orthogonal-matrix.md) has determinant $+1$. It is therefore a genuine [rotation in three dimensions](../../../../../rotation-in-three-dimensions.md), proving sufficiency rather than just spherical [isometry](../../../../../isometry.md).

For the [circle](../../../../../circle.md) assertion, a nondegenerate [generalized circle](../../../../../generalized-circle-under-a-mobius-transformation.md) has an equation

$$
A|z|^2+Bz+\overline B\,\overline z+C=0,
\qquad A,C\in\mathbb R,\quad |B|^2-AC>0.
$$

For $A\ne0$ this is an ordinary [circle](../../../../../circle.md), and for $A=0$ it is a line with infinity included. On the [sphere](../../../../../sphere.md) write coordinates $(p_1,p_2,p_3)$, with $z=(p_1+ip_2)/(1-p_3)$ and $|z|^2=(1+p_3)/(1-p_3)$. Multiplication by $1-p_3$ gives the plane

$$
2\operatorname{Re}B\,p_1-2\operatorname{Im}B\,p_2+(A-C)p_3+(A+C)=0.
$$

If $n=(2\operatorname{Re}B,-2\operatorname{Im}B,A-C)$ and $h=-(A+C)$, then $|n|^2-h^2=4(|B|^2-AC)>0$. Thus the plane intersects the unit [sphere](../../../../../sphere.md) in a proper [circle](../../../../../circle.md). It contains the north pole exactly when $A=0$, accounting for the point at infinity on a line.

Conversely, a [circle](../../../../../circle.md) on the [sphere](../../../../../sphere.md) is the intersection with a plane $n\cdot p=h$, $|h|<|n|$. Set $A=(n_3-h)/2$, $C=(-n_3-h)/2$ and $B=(n_1-in_2)/2$. The preceding equation is recovered and has $|B|^2-AC=(|n|^2-h^2)/4>0$. Its inverse stereographic image is an ordinary [circle](../../../../../circle.md) or a line with infinity attached. This proves both directions of the [circle-plane relation under stereographic projection](../../../../../circle-plane-relation-under-stereographic-projection.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
