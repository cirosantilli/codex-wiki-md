<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Retain the [material frame indifference](../../../../material-frame-indifference.md) assumption used in part (c), in addition to [material isotropy](../../../../material-isotropy.md). Put $p=u_{,1}$, $q=u_{,2}$ and $s=p^2+q^2$. For this [antiplane shear](../../../../antiplane-shear.md),

$$
F=\begin{pmatrix}1&0&0\\0&1&0\\p&q&1\end{pmatrix},\qquad
B=\begin{pmatrix}1&0&p\\0&1&q\\p&q&1+s\end{pmatrix},\qquad J=1.
$$

The invariant identities give $I_B=II_B=3+s$ and $III_B=1$. Hence the restriction of the [strain energy density](../../../../strain-energy-density.md) is

$$
\boxed{W(Dy)=w(|Du|^2),\qquad w(s)=h(3+s,3+s,1).}
$$

[Antiplane energy does not determine the full stress](../../../../antiplane-energy-does-not-determine-the-full-stress.md): the restriction gives one [scalar](../../../../scalar.md) energy along antiplane gradients. It does not determine the full [stress](../../../../stress.md) derivative with respect to every entry of $F$.

Indeed, using the [isotropic hyperelastic stress invariant representation](../../../../isotropic-hyperelastic-stress-invariant-representation.md) and differentiating the energy, with $h_j$ denoting the corresponding [partial derivatives](../../../../partial-derivative.md), gives

$$
DW=2h_1F+2h_2(I_BI-B)F+2III_Bh_3F^{-T}.
$$

Using $S=J^{-1}TF^T$, the general objective [isotropic](../../../../isotropy.md) [Cauchy stress tensor](../../../../cauchy-stress-tensor.md) is

$$
\boxed{S=\frac2J\left[h_1B+h_2(I_BB-B^2)+III_Bh_3I\right].}
$$

All [derivatives](../../../../derivative.md) are evaluated at the current invariant triple. The extra terms generally remain nonzero on antiplane gradients, so **the printed assertion that the full [stress](../../../../stress.md) must be $\beta B$ does not follow**.

A stress-free, objective [isotropic](../../../../isotropy.md) counterexample is the compressible [neo-Hookean solid](../../../../neo-hookean-solid.md) $W(F)=\frac\mu2(|F|^2-3)-\mu\log J$, with $\mu>0$. Its derivative is $T=\mu F-\mu F^{-T}$, so on antiplane gradients

$$
S=\mu(B-I).
$$

Take $u(x_1,x_2)=x_1$. Then $B_{22}=1$ but $S_{22}=0$, whereas $B_{13}=1$ and $S_{13}=\mu$. The diagonal entry would force $\beta=0$, contradicting the shear entry. Thus this is not a matter of choosing the right [scalar](../../../../scalar.md) coefficient.

For the additional one-invariant constitutive assumption $W(F)=\widehat w(I_B)$, the stronger formula does hold, with

$$
\boxed{\beta(I_B,III_B)=\frac{2\widehat w'(I_B)}{\sqrt{III_B}}.}
$$

This is a valid special case, rather than a consequence of [material isotropy](../../../../material-isotropy.md) alone. For the general restricted energy, the shear entries are still fixed: $S_{31}=2w'(s)u_{,1}$ and $S_{32}=2w'(s)u_{,2}$, since $w'=h_1+h_2$ along $(3+s,3+s,1)$. The full [normal stress](../../../../normal-stress.md) needs the constitutive information that the printed claim omits. If [material isotropy](../../../../material-isotropy.md) alone is interpreted without [material frame indifference](../../../../material-frame-indifference.md), even the first reduction to $|Du|^2$ needs that additional [material frame indifference](../../../../material-frame-indifference.md) assumption.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
