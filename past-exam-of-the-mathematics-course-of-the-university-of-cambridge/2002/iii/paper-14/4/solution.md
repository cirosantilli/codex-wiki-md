<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A rank-$k$ [complex vector bundle](../../../../../complex-vector-bundle.md) is a smooth map $\pi:E\to B$ whose fibers are $k$-dimensional complex [vector spaces](../../../../../vector-space-split.md), with local [diffeomorphisms](../../../../../diffeomorphism.md) $\Phi_i:\pi^{-1}(U_i)\to U_i\times\mathbb C^k$ commuting with projection and linear on every fiber. Define [transition functions of a vector bundle](../../../../../transition-function-of-a-vector-bundle.md) by

$$
\Phi_i\Phi_j^{-1}(b,v)=(b,g_{ij}(b)v),\qquad g_{ij}:U_i\cap U_j\to GL(k,\mathbb C).
$$

They are smooth and obey

$$
\boxed{g_{ii}=I,\qquad g_{ij}=g_{ji}^{-1},\qquad g_{ij}g_{jk}=g_{ik}}
$$

on the appropriate double/triple overlaps. The [structure group of a vector bundle](../../../../../structure-group-of-a-vector-bundle.md) is a Lie subgroup $G\subset GL(k,\mathbb C)$ in which a chosen set of transitions takes values. It records allowed changes of fiber frame; different trivializations may exhibit different reductions of that group.

Using the same cocycle, glue the disjoint union of $U_i\times G$ by

$$
(b,h)_j\sim(b,g_{ij}(b)h)_i.
$$

The cocycle makes this an equivalence relation and makes its local charts compatible. Right multiplication $(b,h)_i\cdot a=(b,ha)_i$ is well-defined because it commutes with the left gluing [matrices](../../../../../matrix.md). It is free and transitive on each fiber. These charts therefore construct the associated right [principal bundle](../../../../../principal-bundle.md) $P\to B$ with group $G$.

For the natural line realization, take the [complex tautological line bundle](../../../../../complex-tautological-line-bundle.md) $L=\{(\ell,v):\ell\in\mathbb{CP}^1,\ v\in\ell\subset\mathbb C^2\}$. Its nonzero vectors identify with $\mathbb C^2\setminus\{0\}$ by $(\ell,v)\mapsto v$, with projection $v\mapsto[v]$. On the two standard charts, use $\zeta=z_2/z_1$ and $\eta=z_1/z_2=1/\zeta$. The local frames are $e_0=(1,\zeta)$ and $e_1=(\eta,1)$, so $e_1=e_0/\zeta$. Normalize them using the ambient Hermitian norm:

$$
u_0=\frac{(1,\zeta)}{\sqrt{1+|\zeta|^2}},\qquad
u_1=\frac{(\eta,1)}{\sqrt{1+|\eta|^2}}
=\frac{|\zeta|}{\zeta}u_0.
$$

If $v=t_0u_0=t_1u_1$, then $t_0=(|\zeta|/\zeta)t_1$. Thus the [unitary transitions of the tautological line over the projective line](../../../../../unitary-transitions-of-the-tautological-line-over-the-projective-line.md) are

$$
\boxed{g_{01}(\zeta)=\frac{|\zeta|}{\zeta}\in S^1,\qquad
g_{10}=g_{01}^{-1},\qquad g_{00}=g_{11}=1}.
$$

These are smooth on the overlap $\zeta\ne0$. A [Hermitian metric on a smooth complex vector bundle](../../../../../hermitian-metric-on-a-smooth-complex-vector-bundle.md) generally permits precisely this unitary reduction; here the ambient norm supplies it explicitly.

The corresponding principal circle bundle consists of unit vectors in the tautological line. Sending $(\ell,v)$ to $v$ identifies its total space with $S^3\subset\mathbb C^2$, and the right circle action is $v\cdot e^{i\theta}=e^{i\theta}v$. Identify $\mathbb{CP}^1$ with $S^2$ using

$$
[z_1:z_2]\longmapsto
\frac{(2\operatorname{Re}(z_1\bar z_2),\ 2\operatorname{Im}(z_1\bar z_2),\ |z_1|^2-|z_2|^2)}{|z_1|^2+|z_2|^2}.
$$

Its affine-coordinate inverse on the chart $Z\ne-1$ is $\zeta=(X-iY)/(1+Z)$; the other chart handles the missing pole. This gives a [diffeomorphism](../../../../../diffeomorphism.md), and the projection becomes the [Hopf fibration](../../../../../hopf-fibration.md)

$$
\boxed{S^3\longrightarrow S^2,\qquad
(z_1,z_2)\longmapsto(2\operatorname{Re}(z_1\bar z_2),2\operatorname{Im}(z_1\bar z_2),|z_1|^2-|z_2|^2)}.
$$

There is a distinction if the stated punctured-bundle identification is interpreted only as a projection-preserving [diffeomorphism](../../../../../diffeomorphism.md), rather than a fiber-linear identification. It does not determine whether the complex line is tautological or dual: for a nonzero $\phi\in L_\ell^*$, the unique $v\in\ell$ with $\phi(v)=1$ gives a smooth map $L^*\setminus0\to L\setminus0$. Locally it is inversion of a nonzero complex number. Thus [punctured line bundles do not determine their duality sign](../../../../../punctured-line-bundles-do-not-determine-their-duality-sign.md).

For completeness, these are the only possible signs here. Complex line bundles over $S^2$ are described by the [clutching construction](../../../../../clutching-construction.md) with a loop in $\mathbb C^*$, reducible to $S^1$, and its integer [winding number](../../../../../winding-number.md) determines the bundle: a zero-degree ratio has a logarithm and can be removed by changes of trivializations extending over the two disks. For [winding number](../../../../../winding-number.md) $d$, the unit circle bundle has [fundamental group](../../../../../fundamental-group.md) $\mathbb Z/d\mathbb Z$, as the two solid-torus trivializations identify the common fiber generator and impose its $d$th power as the equatorial gluing relation. There is a fiberwise radial [deformation retraction](../../../../../deformation-retraction.md) from the punctured [line bundle](../../../../../line-bundle.md) onto its unit circle bundle. Since $\mathbb C^2\setminus0$ retracts to [simply connected](../../../../../simply-connected-space.md) $S^3$, the hypothesis forces $|d|=1$.

Consequently the allowed unitary transitions are the displayed $g_{01}$ or its reciprocal, according to the bundle's sign. For the dual, the same underlying Hopf projection has the inverse principal action $v\cdot e^{i\theta}=e^{-i\theta}v$. **In either case the principal total space and projection are $S^3\to S^2$; the purely diffeomorphic hypothesis alone leaves the circle-action sign unspecified**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
