<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The original PDF has a sign defect in the lower-left stage coefficient.** Put $d=c_2-c_1$. With the printed negative sign, the row sums and the relevant [Butcher order conditions](../../../../../../butcher-order-condition.md) are

$$
Ae=\begin{pmatrix}c_1\\-c_1c_2/d\end{pmatrix},\qquad
b^Te=1,\quad b^Tc=\tfrac12,\quad
q:=b^TAe=\tfrac12-\frac{(\tfrac12-c_1)c_2^2}{d^2}.
$$

Thus the claimed universal second order is false. For example $c_1=0,c_2=1$ gives, on $y'=y$, two stages equal to $y$ and the update $Y=(1+h)y$. This is the first-order [Forward Euler method](../../../../../../euler-method.md). For the literal tableau, order at least two holds exactly when $c_1=1/2$ or $c_2=0$, subject to distinct allowed nodes.

For completeness the literal tableau's [A-stability](../../../../../../a-stability.md) can also be classified algebraically. Define

$$
a=\frac{c_1+c_2}{2}>0,\qquad
D=\frac{c_1c_2}{2}\left(1-\frac{c_1c_2}{d^2}\right),\qquad
r=D+q-a.
$$

The [stability function](../../../../../../stability-function.md) obtained from $R(z)=1+zb^T(I-zA)^{-1}e$ is

$$
R(z)=\frac{1+(1-a)z+rz^2}{1-az+Dz^2}.
$$

If $D\geq0$, the denominator has no zero in the closed left half-plane: its reciprocal roots are the stage-matrix [eigenvalues](../../../../../../eigenvalue.md), whose positive sum and nonnegative product give positive real parts for nonzero [eigenvalues](../../../../../../eigenvalue.md). On the imaginary axis,

$$
|1-aiy+D(iy)^2|^2-|1+(1-a)iy+r(iy)^2|^2
=(2q-1)y^2+(D^2-r^2)y^4.
$$

Consequently **for the literal tableau with uniquely solvable stages throughout the left half-plane, the complete parameter criterion is**

$$
\boxed{D\geq0,\qquad q\geq\tfrac12,\qquad D^2\geq(D+q-a)^2.}
$$

These explicit inequalities in $c_1,c_2$ are necessary by the small and large imaginary parameters, and sufficient by the [maximum modulus principle](../../../../../../maximum-modulus-principle.md), including the bound at infinity. For $D=0$ the last inequality forces $r=0$, leaving the stable linear-fractional case. For $D<0$ there is a negative real stage pole. If one defines [stability](../../../../../../stability-of-a-numerical-method.md) solely through an analytically continued scalar [stability function](../../../../../../stability-function.md), the only additional possibilities are

$$
D=q(a-q),\qquad q>a,\qquad q\geq\tfrac12.
$$

Indeed these are precisely the cases where the left pole cancels and $R(z)=[1+(1-q)z]/[1-qz]$ is an [A-stable](../../../../../../a-stability.md) [theta method](../../../../../../theta-method.md). The original stage equations are nevertheless singular at $z=-1/(q-a)$, so they do not give uniquely determined stages there. This distinction prevents a canceled rational factor from concealing an ill-defined stage solve.

The natural intended repair is to replace just the lower-left coefficient by $+c_2^2/(2d)$. This makes the method the [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) on the two nodes. To derive the repaired entries, take

$$
L_1(t)=\frac{c_2-t}{d},\qquad L_2(t)=\frac{t-c_1}{d},\qquad
 a_{ij}=\int_0^{c_i}L_j(t)\,dt,\quad b_j=\int_0^1L_j(t)\,dt.
$$

Integration gives the other three printed entries and the weights unchanged, with the positive lower-left entry. Since $L_1+L_2=1$ and $c_1L_1+c_2L_2=t$, it follows that $Ae=c$, $b^Te=1$ and $b^Tc=1/2$. Hence **the corrected family is always of order at least two**.

For the corrected family let $a=(c_1+c_2)/2$, $D=c_1c_2/2$ and $r=(1-c_1)(1-c_2)/2$. Its [stability function](../../../../../../stability-function.md) has the same displayed rational form, now with $q=1/2$. The denominator again has no left-half-plane zero, and on the imaginary axis the squared-modulus difference is $(D^2-r^2)y^4$. Because $D,r\geq0$, the necessary and sufficient inequality is $D\geq r$, or

$$
\boxed{c_1+c_2\geq1\quad\text{for the corrected two-node collocation family}.}
$$

For sufficiency, $|R|\leq1$ on the imaginary axis and at infinity; apply the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) on growing left half-discs to get the same bound inside. If $D=0$, the condition leaves the endpoint [trapezoidal rule](../../../../../../trapezoidal-rule.md) and its linear denominator. If $c_1+c_2<1$, every nonzero imaginary argument gives $|R|>1$. This is the [two-node collocation A-stability criterion](../../../../../../two-node-collocation-a-stability-criterion.md), explicitly distinguished from the literal defective tableau.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
