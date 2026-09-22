<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

There is an exact rational-map description of [sigma-model lumps](../../../../../sigma-model-lump.md) and a restricted variational rational-map description of [Skyrmions](../../../../../skyrmion.md). The first follows from a [Bogomolny equation](../../../../../bogomolny-equations.md); the second separates angular and radial dependence in a field that generally does not saturate a [Bogomolny bound](../../../../../bogomolny-bound.md).

For the exact example, take the two-dimensional [O3 nonlinear sigma model](../../../../../o3-nonlinear-sigma-model.md) with a unit field $\mathbf n$, energy $E=\frac12\int|\nabla\mathbf n|^2d^2x$, and a fixed limit at infinity. Regular fields then have a [one-point compactification](../../../../../alexandroff-extension.md) to maps $S^2\to S^2$. Choose the orientation so that the stereographic field

$$
u=\frac{n_1+in_2}{1+n_3},\qquad z=x+iy,
$$

has positive charge when it is [holomorphic](../../../../../complex-differentiability-at-a-point.md). Equivalently, this is the [CP1 nonlinear sigma model](../../../../../o3-nonlinear-sigma-model.md) since the target sphere is the [complex projective line](../../../../../complex-projective-line.md). Its energy and [topological charge](../../../../../topological-charge.md) are

$$
E=4\int\frac{|u_z|^2+|u_{\bar z}|^2}{(1+|u|^2)^2}\,d^2x,
\qquad
N=\frac1\pi\int\frac{|u_z|^2-|u_{\bar z}|^2}{(1+|u|^2)^2}\,d^2x.
$$

Subtracting $4\pi N$ gives $8\int|u_{\bar z}|^2/(1+|u|^2)^2$, so for $N>0$,

$$
\boxed{E\geq4\pi N,\qquad u_{\bar z}=0\text{ at equality}.}
$$

The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) therefore give the minimal-energy fields. A [holomorphic map](../../../../../holomorphic-map.md) from the compactified domain [Riemann sphere](../../../../../riemann-sphere.md) to the target [Riemann sphere](../../../../../riemann-sphere.md) is a [rational map](../../../../../rational-map-complex-analysis.md) $u=p(z)/q(z)$, with common [polynomial factors](../../../../../polynomial-factor.md) cancelled. Its [degree of a rational map of the Riemann sphere](../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md) is $N=\max(\deg p,\deg q)$. Poles of $u$ are coordinate singularities, not singularities of $\mathbf n$. For instance, $u=(z-a)/\lambda$ with $\lambda\ne0$ is an exact unit lump with energy $4\pi$, arbitrary centre $a$, and scale $|\lambda|$. Its density is $4|\lambda|^2/(|z-a|^2+|\lambda|^2)^2$, whose plane [integral](../../../../../integral.md) is $4\pi$. For negative charge use antiholomorphic maps. Scale invariance allows arbitrarily small lumps and does not by itself prevent a singular concentration limit in the time-dependent theory.

The local angular geometry of any degree-$N$ [rational map](../../../../../rational-map-complex-analysis.md) is measured by its [angular Jacobian of a rational map](../../../../../angular-jacobian-of-a-rational-map.md),

$$
J_R(z)=\left[\frac{1+|z|^2}{1+|R|^2}|R'|\right]^2,
\qquad R^*d\Omega=J_Rd\Omega,\qquad\int_{S^2}J_Rd\Omega=4\pi N.
$$

For $R=p/q$, the [Wronskian of a rational map](../../../../../wronskian-of-a-rational-map.md) is

$$
\boxed{W(z)=p'(z)q(z)-p(z)q'(z),\qquad R'=\frac{W}{q^2}.}
$$

At ordinary finite points its zeros mark [ramification points of a holomorphic map](../../../../../ramification-point-of-a-holomorphic-map.md), where the angular density vanishes. At a pole use $q/p$ as the target coordinate, and at infinity use $1/z$ as the domain coordinate. A pole of order $m$ is ramified by $m-1$. The [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) counts total ramification $2N-2$, including infinity, even if the affine [Wronskian](../../../../../wronskian.md) has smaller degree. For $R=z^N$, $W=Nz^{N-1}$ accounts for $N-1$ zeros at zero; the reciprocal coordinate shows the other $N-1$ at infinity.

For the approximate example, the [rational map approximation for Skyrmions](../../../../../rational-map-approximation-for-skyrmions.md) uses spherical radius $r$, angular [stereographic projection](../../../../../stereographic-projection.md) coordinate $z$, and

$$
U(r,z)=\cos f(r)+i\sin f(r)\mathbf n_R(z)\cdot\boldsymbol\sigma,
\qquad
\mathbf n_R=\frac{(2\operatorname{Re}R,2\operatorname{Im}R,1-|R|^2)}{1+|R|^2},
\quad f(0)=\pi,quad f(\infty)=0.
$$

The [Pauli matrices](../../../../../pauli-matrices.md) make this an [SU(2) group](../../../../../su-2-group.md)-valued field. The boundary conditions give a continuous centre and the vacuum value at infinity; the profile must also make the energy finite. Angular degree and radial winding factorize to give

$$
\boxed{B=-\frac{2N}{\pi}\int_0^\infty f'\sin^2f\,dr=N.}
$$

At radii with nonzero $-f'\sin^2f$, the angular [baryon number](../../../../../baryon-number.md) density is proportional to $J_R$. Thus the [Wronskian of a rational map](../../../../../wronskian-of-a-rational-map.md) locates zero-density directions and reveals the holes or face directions in shell-like Skyrmion configurations.

In dimensionless [Skyrme model](../../../../../skyrme-model.md) units, insert this ansatz into the quadratic and quartic derivative energies. The angular terms integrate to $4\pi N$ or to the [angular integral in the rational map approximation](../../../../../angular-integral-in-the-rational-map-approximation.md),

$$
\mathcal I[R]=\frac1{4\pi}\int_{S^2}J_R^2d\Omega,
\qquad
E=4\pi\int_0^\infty\left[r^2f'^2+2N(f'^2+1)\sin^2f+\mathcal I\frac{\sin^4f}{r^2}\right]dr.
$$

First minimize $\mathcal I$ over degree-$N$ maps, then solve the radial variational equation

$$
(r^2+2N\sin^2f)f''+2rf'+N\sin(2f)(f'^2-1)-\frac{\mathcal I}{r^2}\sin^2f\sin(2f)=0
$$

with the stated boundary conditions. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\mathcal I\geq N^2$ because $J_R$ has sphere average $N$. For $N=1$ an isometric map such as $R=z$ has $J_R=1$, $\mathcal I=1$, and reduces to the [Skyrmion hedgehog ansatz](../../../../../skyrmion-hedgehog-ansatz.md); its profile still requires solving the radial equation. For general $N$, angular and radial separation restrict the allowed fields. The minimum within this class is an upper bound on the full sector minimum, not a claim that every exact Skyrmion has this separated form. The original construction is Houghton, Manton and Sutcliffe's [https://arxiv.org/abs/hep-th/9705151.](https://arxiv.org/abs/hep-th/9705151.)

A [rotational symmetry of a rational map](../../../../../rotational-symmetry-of-a-rational-map.md) must satisfy $R(gz)=hR(z)$, where $g,h$ are the domain and target rotations written as [Möbius transformations](../../../../../mobius-transformation.md) from [SU(2) matrices](../../../../../su-2-matrix.md). Since a target rotation is an [isometry](../../../../../isometry.md), this identity implies $J_R(gz)=J_R(z)$. For $R=z^N$, $R(e^{i\alpha}z)=e^{iN\alpha}R(z)$, giving axial spatial symmetry accompanied by an internal rotation. This explains the axial symmetry of the degree-two toroidal ansatz.

A useful degree-four example is

$$
R(z)=\frac{z^4+2\sqrt3\,iz^2+1}{z^4-2\sqrt3\,iz^2+1},\qquad
W(z)=8\sqrt3\,iz(1-z^4).
$$

Its finite ramification directions are $0,\pm1,\pm i$, with the sixth at infinity. They are the six coordinate-axis directions under [stereographic projection](../../../../../stereographic-projection.md), so they are the face normals of a cube. The full map has octahedral rotational equivariance: for example $R(iz)=1/R(z)$, and the cyclic-axis generator $g(z)=(iz+1)/(1-iz)$ obeys $R(gz)=e^{2\pi i/3}R(z)$. These generate the cube's rotational group and give a cubic angular density. The associated profile then produces the familiar cubic charge-four approximation. Symmetry of the [Wronskian](../../../../../wronskian.md) is a useful necessary diagnostic but is not sufficient: replacing this map by $cR$, $c>0$, leaves the same ramification directions, while the identity under $z\mapsto iz$ becomes $cR(iz)=c^2/(cR(z))$, whose target transformation is a sphere rotation only when $c=1$. Equivariance of the entire rational map, rather than symmetry of its critical-point set alone, determines the physical rotational symmetry.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
