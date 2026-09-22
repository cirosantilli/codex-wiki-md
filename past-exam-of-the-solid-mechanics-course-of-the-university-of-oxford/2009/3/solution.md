<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [material symmetry group](../../../material-symmetry-group.md) consists of invertible admissible reference transformations $H$ for which $W(FH)=W(F)$ for every admissible $F$. Its rotational part lies in $SO(3)$; a [determinant](../../../determinant.md)-one reference convention restricts the full group to the corresponding special linear group. This right action is distinct from the spatial left action $W(QF)=W(F)$ of [material frame indifference](../../../material-frame-indifference.md).

The proper cube-rotation group has $\boxed{24}$ elements. Choose the image of one outward face normal in six ways, then the image of an adjacent perpendicular normal in four ways; orientation fixes the third direction. No reflections are included. For an isotropic material every proper rotation belongs to the [material symmetry group](../../../material-symmetry-group.md).

Combine [material isotropy](../../../material-isotropy.md) with the physical frame-indifference condition. The [singular value decomposition](../../../singular-value-decomposition.md) may be written $F=R\operatorname{diag}(v_1,v_2,v_3)Q$ with $R,Q\in SO(3)$ because $\det F>0$. Left and right rotational invariance remove $R,Q$. Signed permutation rotations permit any permutation of the three diagonal stretches, so

$$
\boxed{W(F)=\Phi(v_1,v_2,v_3),\qquad\Phi\text{ symmetric in its three arguments}.}
$$

Right invariance alone, without the usual [material frame indifference](../../../material-frame-indifference.md) assumption, would not suffice to remove spatial orientation.

The strict [Baker-Ericksen inequalities](../../../baker-ericksen-inequalities.md) say that larger distinct principal stretches carry larger principal Cauchy stresses:

$$
\boxed{(\sigma_i-\sigma_j)(v_i-v_j)>0\quad\text{if }v_i\ne v_j,\qquad
\sigma_i=J^{-1}v_i\Phi_i.}
$$

A [natural state of a hyperelastic material](../../../natural-state-of-a-hyperelastic-material.md) has zero stress. If two stretches differed, their equal zero stresses would contradict the strict inequality. Thus all three equal some $v>0$, and [polar decomposition](../../../polar-decomposition.md) gives $\boxed{F=vQ}$, $Q\in SO(3)$. A weak non-strict inequality alone would not prove this conclusion, so its strict convention is explicit here.

For the radial deformation put $f(R)=r(R)/R$, $R=|\mathbf x|$, $\boldsymbol\theta=\mathbf x/R$. Since $\partial_jR=\theta_j$,

$$
D\mathbf y=fI+Rf'\boldsymbol\theta\otimes\boldsymbol\theta
=\boxed{\frac rR I+\left(r'-\frac rR\right)\boldsymbol\theta\otimes\boldsymbol\theta.}
$$

This symmetric tensor has radial [eigenvalue](../../../eigenvalue.md) $r'$ and the repeated tangential [eigenvalue](../../../eigenvalue.md) $r/R$. Both are positive in the open annulus under the stated monotonicity/nonnegativity conditions. Therefore these are its principal stretches. The two cases below establish [radial zero-energy rigidity](../../../radial-zero-energy-rigidity.md) by different arguments.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2009](../../2009-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
