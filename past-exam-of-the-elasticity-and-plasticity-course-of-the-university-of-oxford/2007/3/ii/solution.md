<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $e_{xx}=u_{x,x}$, $e_{yy}=u_{y,y}$ and $2e_{xy}=u_{x,y}+u_{y,x}$. Differentiating twice and cancelling the [mixed partial derivatives](../../../../mixed-partial-derivative.md) gives

$$
\boxed{e_{xx,yy}-2e_{xy,xy}+e_{yy,xx}=0.}
$$

A convenient set of six three-dimensional [Saint-Venant compatibility equations](../../../../saint-venant-strain-compatibility-and-differential-identities.md) is

$$
\boxed{\begin{aligned}
e_{11,22}+e_{22,11}-2e_{12,12}&=0,\\
e_{22,33}+e_{33,22}-2e_{23,23}&=0,\\
e_{33,11}+e_{11,33}-2e_{13,13}&=0,\\
e_{11,23}+e_{23,11}-e_{12,13}-e_{13,12}&=0,\\
e_{22,13}+e_{13,22}-e_{12,23}-e_{23,12}&=0,\\
e_{33,12}+e_{12,33}-e_{13,23}-e_{23,13}&=0.
\end{aligned}}
$$

They follow by inserting $e_{ij}=(u_{i,j}+u_{j,i})/2$ and commuting [derivatives](../../../../derivative.md). They form the six symmetric components of the incompatibility [tensor](../../../../tensor.md) $C_{ij}=\epsilon_{ik\ell}\epsilon_{jmn}e_{\ell n,km}$, up to the indicated signs and permutation of components.

They obey the three differential identities $\partial_iC_{ij}=0$, because a symmetric pair of [derivatives](../../../../derivative.md) contracts with an antisymmetric [Levi-Civita symbol](../../../../levi-civita-symbol.md). Thus **there are three independent differential constraints**, represented symmetrically by six component equations; they are not six unrelated constraints on the six [strain](../../../../strain.md) functions. For example, at a nonzero [wavevector](../../../../wavevector.md) directed along the third axis, compatibility imposes $e_{11}=e_{22}=e_{12}=0$ while $e_{13},e_{23},e_{33}$ can arise from the three [displacement](../../../../displacement.md) components. This confirms [rank](../../../../rank-one-quadratic-form.md) three. One cannot simply discard the same arbitrary three component equations in every direction; their independence is differential, with the stated identities. On a [simply connected](../../../../simply-connected-space.md) domain these are the local [Saint-Venant compatibility equations](../../../../saint-venant-strain-compatibility-and-differential-identities.md) for [strain](../../../../strain.md) to be a symmetric [displacement](../../../../displacement.md) [gradient](../../../../gradient.md), while domains that are [multiply connected regions](../../../../multiply-connected-region.md) require global closure conditions as in the screw example. This is [Saint-Venant strain compatibility and differential identities](../../../../saint-venant-strain-compatibility-and-differential-identities.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
