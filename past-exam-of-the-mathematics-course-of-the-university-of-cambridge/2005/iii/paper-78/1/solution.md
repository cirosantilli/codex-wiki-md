<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [polar decomposition of an invertible real matrix](../../../../../polar-decomposition-of-an-invertible-real-matrix.md), start with $C=F^TF$. For nonzero $y$, $y^TCy=|Fy|^2>0$, since $\det F>0$ makes $F$ invertible. The [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives an [orthonormal basis](../../../../../orthonormal-basis.md) $n_a$ with $Cn_a=\lambda_a^2n_a$ and $\lambda_a>0$. Define

$$
U=\sum_a\lambda_a n_a\otimes n_a,\qquad R=FU^{-1}.
$$

Then $U$ is a [positive-definite symmetric matrix](../../../../../symmetric-positive-definite-matrix.md), $U^2=C$, and

$$
R^TR=U^{-1}F^TFU^{-1}=I,\qquad
\det R=\frac{\det F}{\det U}=1,
$$

because $\det U=\sqrt{\det(F^TF)}=\det F$. Thus $R$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) with positive determinant. Set $V=RUR^T$; it too is a [positive-definite symmetric matrix](../../../../../symmetric-positive-definite-matrix.md), and $VR=RU=F$. Moreover $V^2=FF^T$. This proves

$$
\boxed{F=RU=VR,\quad U=(F^TF)^{1/2},\quad V=(FF^T)^{1/2},\quad R^TR=I,\quad\det R=1.}
$$

The positive square root is unique: any positive symmetric square root of $C$ commutes with $C$, preserves its eigenspaces and has the positive scalar square root on each of them. Hence $U$, then $R$ and $V$, are unique. These are the [right stretch tensor](../../../../../right-stretch-tensor.md), rotation and [left stretch tensor](../../../../../left-stretch-tensor.md) of the [polar decomposition in continuum mechanics](../../../../../polar-decomposition-in-continuum-mechanics.md).

A standard [spectral strain measure](../../../../../spectral-strain-measure.md) is

$$
E^f=f(U)=\sum_a f(\lambda_a)n_a\otimes n_a.
$$

Take $f\in C^1(0,\infty)$, $f(1)=0$ and $f'(1)=1$, with $f$ strictly increasing; the customary stronger condition $f'(\lambda)>0$ gives a regular one-to-one parameterization of all positive [principal stretches](../../../../../principal-stretch.md). The zero condition makes a rigid rotation [strain](../../../../../strain.md) free, monotonicity distinguishes extension from contraction and prevents nonunit stretch from being [strain](../../../../../strain.md) free, and the derivative normalization gives the ordinary infinitesimal [strain](../../../../../strain.md). Indeed, for $F=I+H$,

$$
U=I+\frac{H+H^T}{2}+O(\|H\|^2),\qquad
E^f=\frac{H+H^T}{2}+o(\|H\|).
$$

Under a superposed spatial rotation $F\mapsto QF$, $F^TF$ and hence $E^f$ remain unchanged, giving [material frame indifference](../../../../../material-frame-indifference.md). Choosing $f(\lambda)=\lambda-1$ satisfies all these conditions and gives the [Biot strain tensor](../../../../../biot-strain-tensor.md)

$$
\boxed{E^{(1)}=U-I.}
$$

The meaning of [work-conjugate stress and strain](../../../../../work-conjugate-stress-and-strain.md) here is that a symmetric material [tensor](../../../../../tensor.md) $T^f$ satisfies

$$
T^f:\dot E^f=P_{Ii}\dot F_{iI}
$$

for every admissible rate, with both powers measured per reference volume. To keep the nominal-stress index convention explicit, write $M_{iI}=P_{Ii}$, so $M=P^T$ and the power is $M:\dot F$. Differentiating $F=RU$ gives $\dot F=R(\Omega U+\dot U)$, where $\Omega=R^T\dot R$ is skew. [Conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) gives symmetry of $MF^T$, or equivalently of $R^TMU$. Therefore

$$
\begin{aligned}
M:\dot F
&=\operatorname{tr}((R^TM)^T\Omega U)
 +(R^TM):\dot U\\
&=\operatorname{tr}((R^TMU)^T\Omega)
 +\operatorname{sym}(R^TM):\dot U\\
&=\operatorname{sym}(R^TM):\dot U.
\end{aligned}
$$

The first term vanishes because a symmetric [tensor](../../../../../tensor.md) has zero contraction with a skew [tensor](../../../../../tensor.md). Since $\dot E^{(1)}=\dot U$, the [symmetric Biot stress](../../../../../symmetric-biot-stress.md) is

$$
\boxed{T^{(1)}=\operatorname{sym}(PR)
=\frac12(PR+R^TP^T).}
$$

If the [nominal stress](../../../../../nominal-stress-tensor.md) is instead stored spatial-index first as $M$, the same answer is $\operatorname{sym}(R^TM)$. The symmetrization is essential: $PR$ need not itself be symmetric.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
