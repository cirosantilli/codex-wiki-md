# Paper 309

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_309.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_309.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The outgoing solution obtained from the [retarded fundamental solution](../../../distribution-theory.md#retarded-fundamental-solution) of the [wave equation](../../../wave-equation.md) is

$$
h_{ab}(t,\mathbf x)=4\int
\frac{T_{ab}-\tfrac12\eta_{ab}T}
{|\mathbf x-\mathbf x'|}
\left(t-|\mathbf x-\mathbf x'|,\mathbf x'\right)d^3x'.
$$

In the [radiation zone](../../../electromagnetism.md#radiation-zone), put $r=|\mathbf x|$, $\mathbf n=\mathbf x/r$, and retain the leading $1/r$ term at [retarded time](../../../electromagnetism.md#retarded-time) $u=t-r$. The trace term disappears after applying the [transverse-traceless projector](../../../general-relativity.md#transverse-traceless-projector)

$$
P_{ij}=\delta_{ij}-n_in_j,
\qquad
\Lambda_{ij,kl}=P_{ik}P_{jl}-\frac12P_{ij}P_{kl},
$$

so

$$
h^{\rm TT}_{ij}(t,\mathbf x)
=\frac4r\Lambda_{ij,kl}(\mathbf n)
\int T_{kl}(u,\mathbf x')d^3x'.
$$

Twice using [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), $\partial_aT^{ab}=0$, and integrating by parts gives

$$
\frac{d^2}{du^2}\int T_{00}x_kx_l\,d^3x
=2\int T_{kl}\,d^3x.
$$

The projector removes the trace, so in terms of the [mass quadrupole moment](../../../general-relativity.md#mass-quadrupole-moment)

$$
Q_{kl}=\int\rho
\left(x_kx_l-\frac13\delta_{kl}|\mathbf x|^2\right)d^3x
$$

the far field is

$$
\boxed{h^{\rm TT}_{ij}=\frac2r\Lambda_{ij,kl}\ddot Q_{kl}(u)}.
$$

The [gravitational-wave energy flux](../../../general-relativity.md#gravitational-wave-energy-flux) is

$$
\frac{dP}{d\Omega}
=\frac{r^2}{32\pi}
\left\langle\dot h^{\rm TT}_{ij}\dot h^{\rm TT}_{ij}\right\rangle.
$$

For a trace-free symmetric tensor $A_{ij}$, the [isotropic tensor integral](../../../geometry-and-topology.md#isotropic-tensor-integral) over the observation direction gives

$$
\int \Lambda_{ij,kl}A_{kl}\Lambda_{ij,mn}A_{mn}\,d\Omega
=\frac{8\pi}{5}A_{ij}A_{ij}.
$$

Consequently the standard [quadrupole formula](../../../general-relativity.md#quadrupole-formula), in the units $G=c=1$ used by the paper, is

$$
\boxed{P=\frac15\left\langle\dddot Q_{ij}\dddot Q_{ij}\right\rangle}.
$$

Thus the printed coefficient $4\pi/5$ is inconsistent with the stated definition of $Q_{ij}$ and the standard wave-energy normalization; it appears to be a typographical error.

For the planet, choose its [circular orbit](../../../classical-mechanics.md#circular-orbit) in the $xy$-plane and write $\omega=2\pi/\tau$. With the star treated as fixed,

$$
\mathbf x=R(\cos\omega t,\sin\omega t,0),
$$

and hence

$$
Q_{ij}=MR^2
\begin{pmatrix}
\cos^2\omega t-\tfrac13&\sin\omega t\cos\omega t&0\\
\sin\omega t\cos\omega t&\sin^2\omega t-\tfrac13&0\\
0&0&-\tfrac13
\end{pmatrix}.
$$

Direct differentiation gives

$$
\dddot Q_{ij}\dddot Q_{ij}=32M^2R^4\omega^6,
$$

so

$$
\boxed{P=\frac{32}{5}M^2R^4\omega^6
=\frac{2048\pi^6}{5}\frac{M^2R^4}{\tau^6}}.
$$

Restoring units multiplies this by $G/c^5$. If the printed $4\pi/5$ coefficient is followed literally, the answer is instead $4\pi$ times larger,

$$
\boxed{P_{\rm printed}=\frac{8192\pi^7}{5}\frac{M^2R^4}{\tau^6}}.
$$

For two bodies of comparable mass, $M$ is replaced by the [reduced mass](../../../classical-mechanics.md#reduced-mass) and $R$ by their separation.

## 2

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

At each point, apply the indefinite-signature version of the [Gram-Schmidt process](../../../linear-algebra.md#gram-schmidt-process) to any local coframe, choosing one timelike and three spacelike one-forms. This produces an [orthonormal coframe in spacetime](../../../general-relativity.md#orthonormal-coframe-in-spacetime) $\{\theta^a\}$ satisfying

$$
g=\eta_{ab}\theta^a\otimes\theta^b,
\qquad \eta_{ab}=\operatorname{diag}(-1,1,1,1).
$$

It is unique only up to a local [Lorentz transformation](../../../special-relativity.md#lorentz-transformation). The torsion-free [connection 1-forms](../../../connection-1-form.md) are then determined by [Cartan's first structure equation](../../../connection-1-form.md#cartan-s-first-structure-equation) and [metric compatibility](../../../fiber-bundle.md#metric-compatibility),

$$
d\theta^a+\omega^a{}_b\wedge\theta^b=0,
\qquad \omega_{ab}=-\omega_{ba}.
$$

[Cartan's second structure equation](../../../connection-1-form.md#cartan-s-second-structure-equation) gives the [curvature 2-forms](../../../connection-1-form.md#curvature-2-form)

$$
\mathcal R^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b
=\frac12R^a{}_{bcd}\theta^c\wedge\theta^d,
$$

and contraction gives the [Ricci tensor](../../../general-relativity.md#ricci-tensor) $R_{bd}=R^a{}_{bad}$.

For the displayed metric, take

$$
\theta^0=dt,
\qquad \theta^i=e^{-t}dx^i
\quad(i=1,2,3).
$$

Then $d\theta^0=0$ and $d\theta^i=-\theta^0\wedge\theta^i$. The nonzero connection forms are therefore

$$
\boxed{\omega^i{}_0=-\theta^i,
\qquad \omega^0{}_i=-\theta^i},
$$

with $\omega^i{}_j=0$. A second application of the structure equations gives

$$
\mathcal R^i{}_0=\theta^0\wedge\theta^i,
\qquad
\mathcal R^0{}_i=\theta^0\wedge\theta^i,
\qquad
\mathcal R^i{}_j=\theta^i\wedge\theta^j.
$$

Equivalently,

$$
\boxed{\mathcal R^a{}_b=\theta^a\wedge\theta_b},
$$

so this is a [constant sectional curvature](../../../general-relativity.md#constant-sectional-curvature) spacetime with $K=1$. In four dimensions,

$$
R_{ab}=3g_{ab},
\qquad R=12,
\qquad G_{ab}=R_{ab}-\frac12Rg_{ab}=-3g_{ab}.
$$

The [Vacuum Einstein equations](../../../general-relativity.md#vacuum-einstein-equations) with a [cosmological constant](../../../cosmology.md#cosmological-constant) are $G_{ab}+\Lambda g_{ab}=0$, and hence

$$
\boxed{\Lambda=3}.
$$

The metric is the contracting flat slicing of [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) with curvature radius one.

## 3

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For an affine parameter $\lambda$, the [geodesic Lagrangian](../../../riemannian-geometry.md#geodesic-lagrangian) is

$$
\mathcal L=\frac12\left[-(1+r^2)\dot t^2
+\frac{\dot r^2}{1+r^2}
+r^2\dot\theta^2+r^2\sin^2\theta\,\dot\phi^2\right].
$$

Varying $S=\int\mathcal L\,d\lambda$ gives the [geodesic equations](../../../riemannian-geometry.md#geodesic-equation)

$$
\ddot t+\frac{2r}{1+r^2}\dot r\dot t=0,
$$



$$
\ddot r+r(1+r^2)\dot t^2
-\frac{r}{1+r^2}\dot r^2
-r(1+r^2)(\dot\theta^2+\sin^2\theta\,\dot\phi^2)=0,
$$



$$
\ddot\theta+\frac{2\dot r}{r}\dot\theta
-\sin\theta\cos\theta\,\dot\phi^2=0,
\qquad
\ddot\phi+\frac{2\dot r}{r}\dot\phi
+2\cot\theta\,\dot\theta\dot\phi=0.
$$

The rotational [Killing vector fields](../../../general-relativity.md#killing-vector-field) of the [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) conserve the angular-momentum vector. Its direction is fixed, so every nonradial orbit lies in the plane through the symmetry centre orthogonal to that vector. A spatial rotation can make this the equatorial plane. Equivalently, the initial conditions $\theta=\pi/2$ and $\dot\theta=0$ solve the $\theta$ equation uniquely. This is the [planarity of geodesics in spherical symmetry](../../../general-relativity.md#planarity-of-geodesics-in-spherical-symmetry); a radial geodesic has zero [angular momentum](../../../classical-mechanics.md#angular-momentum) and may be assigned any plane.

<a id="3/image-an-equatorial-geodesic-in-a-spherically-symmetric-spacetime"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-309-equatorial-plane.png)

**[Figure 1](#3/image-an-equatorial-geodesic-in-a-spherically-symmetric-spacetime). An equatorial geodesic in a spherically symmetric spacetime**.

On $\theta=\pi/2$, the cyclic coordinates $t$ and $\phi$ produce [geodesic conserved quantities from Killing vectors](../../../general-relativity.md#geodesic-conserved-quantity-from-a-killing-vector),

$$
\boxed{E=(1+r^2)\dot t,
\qquad L=r^2\dot\phi}.
$$

For a timelike geodesic parametrized by [proper time](../../../special-relativity.md#proper-time), the [proper-time normalization](../../../special-relativity.md#proper-time-normalization) is $g_{ab}\dot x^a\dot x^b=-1$. Substitution of $E$ and $L$ gives the first-order radial equation

$$
\boxed{\dot r^2=E^2-(1+r^2)\left(1+\frac{L^2}{r^2}\right)}.
$$

This is the [timelike geodesic effective potential](../../../general-relativity.md#timelike-geodesic-effective-potential) for static [Anti-de Sitter spacetime](../../../general-relativity.md#anti-de-sitter-spacetime) with curvature radius one.

A geodesic passing through $r=0$ must have $L=0$. If it moves away from the origin, $E>1$, and

$$
\dot r^2=(E^2-1)-r^2.
$$

Taking proper time $s=0$ at departure gives

$$
r(s)=\sqrt{E^2-1}\sin s
\qquad(0\leq s\leq\pi).
$$

It turns around at $s=\pi/2$ and first returns to the origin at

$$
\boxed{\Delta s=\pi}.
$$

This energy-independent refocusing is the characteristic [radial timelike geodesic in anti-de Sitter spacetime](../../../general-relativity.md#radial-timelike-geodesic-in-anti-de-sitter-spacetime) result; for curvature radius $a$, the answer is $\pi a$.

## 4

↑ **Parent:** [Paper 309](paper-309.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the torsion-free [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), cyclically summing the displayed coordinate expression and using $\Gamma^a{}_{bc}=\Gamma^a{}_{cb}$ gives the algebraic [first Bianchi identity](../../../general-relativity.md#first-bianchi-identity)

$$
\boxed{R^a{}_{bcd}+R^a{}_{cdb}+R^a{}_{dbc}=0}.
$$

Apply the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) to three covariant-derivative commutators, or differentiate the coordinate formula in [normal coordinates](../../../general-relativity.md#normal-coordinates). The third-derivative terms and the derivatives of quadratic connection terms cancel cyclically, giving the differential [second Bianchi identity](../../../general-relativity.md#second-bianchi-identity)

$$
\boxed{\nabla_eR^a{}_{bcd}
+\nabla_cR^a{}_{bde}
+\nabla_dR^a{}_{bec}=0}.
$$

Contracting the first and third curvature indices and then contracting once more yields

$$
\nabla^aR_{ab}-\frac12\nabla_bR=0,
$$

or the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity)

$$
\boxed{\nabla^aG_{ab}=0}.
$$

For the metric variation $h_{ab}=\delta g_{ab}$,

$$
\delta\sqrt{-g}=\frac12\sqrt{-g}\,h,
$$

while the two double-divergence terms in the supplied [metric variation of scalar curvature](../../../general-relativity.md#metric-variation-of-scalar-curvature) become a boundary term after [integration by parts for tensor fields](../../../calculus.md#integration-by-parts-for-tensor-fields). The [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action) therefore contributes $G_{ab}+\Lambda g_{ab}$. Varying the [Proca action](../../../electromagnetism.md#proca-action) with respect to the metric gives the [Proca stress-energy tensor](../../../general-relativity.md#proca-stress-energy-tensor), and the full [Einstein-Proca theory](../../../general-relativity.md#einstein-proca-theory) equation is

$$
\boxed{
R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}
=8\pi\left[
F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}
+m^2A_aA_b-\frac12m^2g_{ab}A_cA^c
\right]}.
$$

Since $\delta F_{ab}=2\nabla_{[a}\delta A_{b]}$, variation with respect to $A_b$ and one [integration by parts](../../../calculus.md#integration-by-parts) give the covariant [Proca equation](../../../electromagnetism.md#proca-equation)

$$
\boxed{\nabla_aF^{ab}-m^2A^b=0}.
$$

Taking its [covariant divergence](../../../general-relativity.md#covariant-divergence) gives

$$
m^2\nabla_bA^b=\nabla_b\nabla_aF^{ab}
=\frac12[\nabla_b,\nabla_a]F^{ab}=0,
$$

because the resulting contractions pair the symmetric [Ricci tensor](../../../general-relativity.md#ricci-tensor) with the antisymmetric [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor). Since $m\ne0$, the [Lorenz constraint in Proca theory](../../../electromagnetism.md#lorenz-constraint-in-proca-theory) follows:

$$
\boxed{\nabla_aA^a=0}.
$$

Moreover, $F=dA$ and $d^2=0$, so the [Electromagnetic Bianchi identity](../../../electromagnetism.md#electromagnetic-bianchi-identity) is

$$
\boxed{\nabla_aF_{bc}+\nabla_bF_{ca}+\nabla_cF_{ab}=0}.
$$

Finally, use that identity to differentiate the matter tensor. The result groups naturally as

$$
\nabla^aT_{ab}
=F_b{}^c\left(\nabla^aF_{ac}-m^2A_c\right)
+m^2A_b\nabla_aA^a.
$$

Both terms vanish by the [Proca equation](../../../electromagnetism.md#proca-equation) and its [Lorenz constraint in Proca theory](../../../electromagnetism.md#lorenz-constraint-in-proca-theory). Thus $\nabla^aT_{ab}=0$, exactly as required by the [contracted Bianchi identity](../../../general-relativity.md#contracted-bianchi-identity) applied to the [Einstein field equations](../../../general-relativity.md#einstein-field-equations). The vector equation is therefore consistent with the gravitational equation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
