<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [homogeneous hyperelastic material](../../../../homogeneous-hyperelastic-material.md) has a [strain energy density](../../../../strain-energy-density.md) per unit reference [volume](../../../../volume.md) $W(F)$ depending on the [deformation gradient](../../../../deformation-gradient.md), with no explicit dependence on the [reference configuration](../../../../reference-configuration.md). For orientation-preserving gradients $F\in GL^+(3)$, its first [Piola-Kirchhoff stress tensor](../../../../piola-kirchhoff-stress-tensors.md) is the [derivative](../../../../derivative.md):

$$
\boxed{\widehat T(F)=D_FW(F),\qquad T_{iA}=\frac{\partial W}{\partial F_{iA}}(F).}
$$

Equivalently the infinitesimal stored-energy change is $DW(F)[H]=T:H$. Reference and spatial indices are distinguished here by upper- and lowercase index letters.

The [material symmetry group](../../../../material-symmetry-group.md) may be written $G_W=\{H\in GL^+(3):W(FH)=W(F)\text{ for every }F\in GL^+(3)\}$. A volume-preserving relabelling convention restricts the candidate $H$ to $SL(3)$; the [material isotropy](../../../../material-isotropy.md) criterion is the same. The material has **[material isotropy](../../../../material-isotropy.md)** when $SO(3)\subseteq G_W$, meaning $W(FQ)=W(F)$ for every proper [rotation](../../../../rotation-mathematics.md) $Q$. If only rotational [symmetries](../../../../symmetry-physics.md) are included in the definition of the group, [material isotropy](../../../../material-isotropy.md) means that group equals $SO(3)$. This right-rotation invariance is distinct from [material frame indifference](../../../../material-frame-indifference.md), the left-rotation invariance $W(QF)=W(F)$.

The [polar decomposition in continuum mechanics](../../../../polar-decomposition-in-continuum-mechanics.md) gives the unique factorizations

$$
\boxed{F=RU=VR,\qquad R\in SO(3),\quad U=(F^TF)^{1/2},\quad V=(FF^T)^{1/2},}
$$

where $U,V$ are [positive-definite symmetric matrices](../../../../symmetric-positive-definite-matrix.md). Their common positive [eigenvalues](../../../../eigenvalue.md) $\lambda_1,\lambda_2,\lambda_3$ are the **[principal stretches](../../../../principal-stretch.md)**, equivalently the [singular values](../../../../singular-value.md) of $F$. They describe the local stretch magnitudes after separating out a rigid [rotation](../../../../rotation-mathematics.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
