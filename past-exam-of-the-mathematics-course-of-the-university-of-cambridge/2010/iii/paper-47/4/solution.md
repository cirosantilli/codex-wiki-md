<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a gauge-field configuration, spatial symmetry means [symmetry up to gauge transformation](../../../../../symmetry-up-to-gauge-transformation.md): the pullback of the fields by a spatial isometry lies in their original [gauge orbit](../../../../../gauge-orbit.md). In the anti-Hermitian convention,

$$
A^g=gAg^{-1}-dg\,g^{-1},\qquad
\Phi^g=g\Phi g^{-1}.
$$

The potential and charged fields need not be strictly fixed in a particular gauge; their gauge-invariant observables must be fixed.

For example, the Abelian potential $A=Bx\,dy$ describes a uniform magnetic field. Translating $x$ by $a$ adds $Ba\,dy=d(Bay)$, a gauge change, although the potential itself changes. For an axially symmetric vortex $\Phi=f(r)e^{iN\theta}$, $A=a(r)d\theta$, rotation through $\beta$ multiplies $\Phi$ by $e^{iN\beta}$; a constant $U(1)$ transformation compensates. These illustrate why literal invariance of the representative is too strong.

For the ['t Hooft-Polyakov monopole](../../../../../t-hooft-polyakov-monopole.md), a spatial rotation $R\in SO(3)$ has an $SU(2)$ lift $g_R$ with adjoint action $R$. The two lifts differ by a central sign and act identically on adjoint fields. The [hedgehog ansatz for a monopole](../../../../../hedgehog-ansatz-for-a-monopole.md) satisfies

$$
\Phi^a(Rx)=R_{ab}\Phi^b(x),\qquad
(R^*A)_i^a(x)=R_{ji}A_j^a(Rx)=R_{ab}A_i^b(x).
$$

The second identity follows from invariance of $\epsilon_{iaj}$ under simultaneous rotations of all three indices. Thus the pulled-back fields are obtained by the constant gauge transformation $g_R$; applying $g_R^{-1}$ restores the representative. In particular $|\Phi|^2$ and the energy density are radial even though $\Phi^a=f(r)x^a/r$ is not literally invariant under rotating space alone.

For the field equations, use the invariant inner product with $[e_a,e_b]=\epsilon_{abc}e_c$. Since $B_i^aB_i^a=\tfrac12F_{ij}^aF_{ij}^a$, a variation $a_j=\delta A_j$, $\psi=\delta\Phi$ gives

$$
\delta V_\lambda
=2\int_{\mathbb R^3}
\left\langle-D_iF_{ij}+[\Phi,D_j\Phi],a_j\right\rangle
-2\left\langle D_iD_i\Phi+\lambda\Phi,\psi\right\rangle\,d^3x.
$$

Here the scalar kinetic contribution to the gauge variation uses  
$\langle D_j\Phi,[a_j,\Phi]\rangle
=\langle[\Phi,D_j\Phi],a_j\rangle$. The [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) for the energy actually printed are

$$
\boxed{D_iF_{ij}=[\Phi,D_j\Phi],\qquad
D_iD_i\Phi+\lambda\Phi=0.}
$$

The PDF has $\lambda(1-|\Phi|^2)$, without a square. This is not the usual nonnegative monopole potential with vacuum $|\Phi|=1$. If the usual $\lambda(1-|\Phi|^2)^2$ were intended, only the scalar equation would change to

$$
D_iD_i\Phi+2\lambda(1-|\Phi|^2)\Phi=0.
$$

The final requested proof at $\lambda=0$ is identical for either interpretation; we do not silently alter the printed energy.

To derive the covariant derivative of the radial fields, first differentiate the Higgs profile:

$$
\partial_k\Phi^a
=\frac fr\delta_{ak}+\frac1r\left(\frac fr\right)'x^ax^k.
$$

The commutator term is

$$
[A_k,\Phi]^a
=\epsilon_{abc}\epsilon_{kbj}x^jx^c\,\frac{\alpha f}{r}
=\frac{\alpha f}{r}(r^2\delta_{ak}-x^ax^k).
$$

Adding the two terms gives exactly

$$
\boxed{D_k\Phi^a=
\left(\frac fr+r\alpha f\right)\delta_{ak}
+\frac1r\left[\left(\frac fr\right)'-\alpha f\right]x^ax^k.}
$$

The radial eigenvalue of the supplied magnetic tensor is $2\alpha+r^2\alpha^2$, while that of this covariant derivative is $f'$. Its transverse coefficients are respectively $r\alpha'+2\alpha$ and $f/r+r\alpha f$. Consequently $B=-D\Phi$ reduces to

$$
\boxed{f'=-2\alpha-r^2\alpha^2,\qquad
r\alpha'+2\alpha=-\frac fr-r\alpha f.}
$$

Equivalently, the [hedgehog monopole equations in radial profile variables](../../../../../hedgehog-monopole-equations-in-radial-profile-variables.md) with $K=1+r^2\alpha$ are

$$
\boxed{K'=-fK,\qquad f'=\frac{1-K^2}{r^2}.}
$$

These are two equations rather than an overdetermined system: radial and transverse projections span the two invariant tensor structures. For a regular monopole in this hedgehog sector, smoothness at the origin gives $f(0)=0$, $K(0)=1$, while the normalized vacuum conditions give $f\to1$, $K\to0$ at infinity; solving the ODEs is not needed here.

Finally, prove that the [Bogomolny monopole equations imply Yang-Mills-Higgs equations](../../../../../bogomolny-monopole-equations-imply-yang-mills-higgs-equations.md), without restricting to the radial ansatz. The three-dimensional [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) is $D_iB_i=0$. If $B_i=-D_i\Phi$, then

$$
D_iD_i\Phi=-D_iB_i=0,
$$

which is the scalar equation at $\lambda=0$. For the gauge equation,

$$
\begin{aligned}
D_iF_{ij}
&=-\epsilon_{ijk}D_iD_k\Phi\\
&=-\frac12\epsilon_{ijk}[F_{ik},\Phi]\\
&=[B_j,\Phi]=[\Phi,D_j\Phi].
\end{aligned}
$$

In the second line antisymmetry eliminates the symmetric derivative part; the curvature commutator is $[D_i,D_k]\Phi=[F_{ik},\Phi]$. The next equality uses  
$\epsilon_{ijk}\epsilon_{ik\ell}=-2\delta_{j\ell}$ and $F_{ik}=\epsilon_{ik\ell}B_\ell$. These are exactly both field equations at $\lambda=0$, so **every smooth Bogomolny solution satisfies them**, not merely those of the hedgehog form.

For finite-energy monopoles, the associated energy argument is also transparent:

$$
V_0=\int|B+D\Phi|^2\,d^3x
-2\int_{S^2_\infty}\langle\Phi,B_i\rangle\,dS_i.
$$

The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) converts $\langle B_i,D_i\Phi\rangle$ into this boundary term. At fixed asymptotic magnetic charge, $B=-D\Phi$ saturates the [Bogomolny bound](../../../../../bogomolny-bound.md). This complements the local differential proof above and explains the energy-minimizing role of the first-order equations.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
