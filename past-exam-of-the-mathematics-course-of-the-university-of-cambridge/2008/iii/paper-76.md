# Paper 76

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper76.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper76.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $b=|\mathbf r_0|$, $r=|\mathbf r|$, $\mathbf P=\mathbf r-\mathbf r_0$ and $P=|\mathbf P|$. Initially assume $0<b<a$ and a nonzero [current dipole](../../../electromagnetism.md#current-dipole). The possible singularities of the continued formulas occur when $r=0$, $P=0$ or

$$
D=rP+\mathbf r\cdot\mathbf P=0.
$$

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $D\geq0$. Away from the two endpoints it vanishes exactly when $\mathbf P$ is antiparallel to $\mathbf r$, namely on the open segment $\mathbf r=s\mathbf r_0$, $0<s<1$. Thus both formulas are regular in the physical exterior $r>a$; the singularities requested here belong to their analytic expressions continued into the sphere.

To determine the order on the segment, let $\mathbf e=\mathbf r_0/b$ and approach an interior point as $\mathbf r=z\mathbf e+\rho\mathbf e_\rho$, with $0<z<b$ and $\mathbf e_\rho\perp\mathbf e$ a unit transverse direction. Expansion gives

$$
D=\frac{b^2\rho^2}{2z(b-z)}+O(\rho^4),
\quad P\mathbf r+r\mathbf P=b\rho\mathbf e_\rho+O(\rho^2),
\quad F=PD=\frac{b^2\rho^2}{2z}+O(\rho^4).
$$

Consequently the leading singular terms in the [electric potential](../../../electromagnetism.md#electric-potential) and [magnetic scalar potential](../../../electromagnetism.md#magnetic-scalar-potential) are

$$
u^+\sim\frac{1}{4\pi\sigma}\frac{2\mathbf Q\cdot\mathbf e_\rho}{b\rho},
\qquad
U\sim\frac{\mu_0}{4\pi}\frac{2z(\mathbf Q\times\mathbf e)\cdot\mathbf e_\rho}{b\rho}.
$$

Thus a dipole with a nonzero transverse moment has **first-order line singularities** on the open segment: their generic growth is $1/\rho$, the inverse distance to that segment. Angular coefficients can vanish along particular approach directions without removing the line singularity.

At the source point put $\mathbf r=\mathbf r_0+P\mathbf n$ with a fixed direction $\mathbf n\neq-\mathbf e$. The explicit dipole term gives

$$
u^+=\frac{2\mathbf Q\cdot\mathbf n}{4\pi\sigma P^2}+O(P^{-1}),
\qquad
U=\frac{\mu_0}{4\pi}\frac{(\mathbf Q\times\mathbf e)\cdot\mathbf n}{P(1+\mathbf e\cdot\mathbf n)}+O(1).
$$

The source therefore has a **second-order electric dipole singularity** and, for a nonradial moment, a **first-order magnetic singularity**. Approaches tangent to the singular segment need not have these fixed-angle scalings.

At the origin put $\mathbf r=r\mathbf n$, with $\mathbf n\neq\mathbf e$. The leading terms are

$$
u^+=\frac{1}{4\pi\sigma}\frac{\mathbf Q\cdot(\mathbf n-\mathbf e)}{br(1-\mathbf n\cdot\mathbf e)}+O(1),
\qquad
U=\frac{\mu_0}{4\pi}\frac{(\mathbf Q\times\mathbf e)\cdot\mathbf n}{b(1-\mathbf n\cdot\mathbf e)}+O(r).
$$

The electric expression has a **first-order point singularity** there. The magnetic expression has a generally direction-dependent finite radial limit, so the origin is a nonremovable endpoint singularity of radial order zero, rather than an isolated $1/r$ pole. It can still be unbounded along approaches whose angle to the segment also tends to zero. Stating the approach matters for this nonisolated singularity.

For a [radial current dipole](../../../electromagnetism.md#radial-current-dipole), $\mathbf Q=q\mathbf e$, the transverse line terms cancel and the electric line singularity is removable. Its only electric singularities are the first-order term $-q/(4\pi\sigma br)$ at the origin and the second-order dipole at $\mathbf r_0$. The magnetic potential is identically zero because $\mathbf Q\times\mathbf r_0=0$. Finally, if $\mathbf r_0=0$, the two terms in the given exterior electric expression combine to

$$
\boxed{u^+=\frac{3}{4\pi\sigma}\frac{\mathbf Q\cdot\mathbf r}{r^3},\qquad U=0.}
$$

There is then just a second-order electric singularity at the origin. A zero dipole moment makes both potentials zero.

## 2

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For this question use the normalized [magnetic scalar potential](../../../electromagnetism.md#magnetic-scalar-potential) $\mathcal U$ defined by $\mathbf B=(\mu_0/4\pi)\nabla\mathcal U$. The previous question instead includes $\mu_0/4\pi$ in its scalar potential; its $U$ equals $(\mu_0/4\pi)\mathcal U$. This normalization change in the paper must be kept separate from the kernel calculation.

Take the radial component of the [Geselowitz formula](../../../electromagnetism.md#geselowitz-formula). On the spherical boundary, $\mathbf n'$ is parallel to $\mathbf r'$, and

$$
[\mathbf n'\times(\mathbf r-\mathbf r')]\cdot\widehat{\mathbf r}=0.
$$

Thus the surface-current term contributes no radial [magnetic field](../../../electromagnetism.md#magnetic-field). The primary [Biot-Savart law](../../../electromagnetism.md#biot-savart-law) term gives, along a fixed direction $\widehat{\mathbf r}$,

$$
\partial_r\mathcal U
=\left[\mathbf Q\times\frac{\mathbf r-\mathbf r_0}{|\mathbf r-\mathbf r_0|^3}\right]\cdot\widehat{\mathbf r}
=-\frac{(\mathbf Q\times\mathbf r_0)\cdot\widehat{\mathbf r}}
{|r\widehat{\mathbf r}-\mathbf r_0|^3}.
$$

Choose $\mathcal U\to0$ at infinity. Integrating this equation fixes the full potential along every ray, giving

$$
\mathcal U=(\mathbf Q\times\mathbf r_0)\cdot\widehat{\mathbf r}
\int_r^\infty\frac{ds}{|s\widehat{\mathbf r}-\mathbf r_0|^3}.
$$

To express it as a source-position derivative, define

$$
\phi(\mathbf r;\mathbf r_0)=\int_r^\infty\frac{ds}{s|s\widehat{\mathbf r}-\mathbf r_0|}.
$$

With $\mathbf W=\mathbf Q\times\mathbf r_0$, differentiating the integrand gives

$$
\mathbf W\cdot\nabla_{\mathbf r_0}\frac1{|s\widehat{\mathbf r}-\mathbf r_0|}
=\frac{s\mathbf W\cdot\widehat{\mathbf r}}{|s\widehat{\mathbf r}-\mathbf r_0|^3},
$$

so $\mathcal U=\mathbf W\cdot\nabla_{\mathbf r_0}\phi$ as required.

Let $b=|\mathbf r_0|$ and $P=|\mathbf r-\mathbf r_0|$. An elementary antiderivative gives the [spherical current-dipole logarithmic kernel](../../../electromagnetism.md#spherical-current-dipole-logarithmic-kernel)

$$
\boxed{\phi(\mathbf r;\mathbf r_0)=\frac1b\log\frac{r+P+b}{r+P-b}.}
$$

For $r>a>b$, both logarithm arguments are positive. Its radial derivative is $-1/(rP)$ and its limit at infinity is zero, which verifies the preceding integral. At $b=0$ use the continuous limit $\phi=1/r$.

For a direct check, differentiating along $\mathbf W$ leaves $b$ unchanged and gives $\mathbf W\cdot\nabla_{\mathbf r_0}P=-\mathbf W\cdot\mathbf r/P$. Since

$$
F=rP^2+P\mathbf r\cdot(\mathbf r-\mathbf r_0)
=\frac P2[(r+P)^2-b^2],
$$

one obtains

$$
\boxed{\mathcal U=\frac{(\mathbf Q\times\mathbf r_0)\cdot\mathbf r}{F}.}
$$

Its gradient is the [Sarvas formula](../../../electromagnetism.md#sarvas-formula). The sphere radius and [electrical conductivity](../../../electromagnetism.md#electrical-conductivity) disappear from this exterior magnetic result because spherical symmetry removed the radial contribution of the return currents. The original derivation and spherical-conductor assumptions are discussed in [Sarvas's paper](https://pubmed.ncbi.nlm.nih.gov/3823129/).

## 3

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Put $\lambda=(r/a)^2$, so the inverted observation point is $\overline{\mathbf r}=\mathbf r/\lambda$ and $\overline r=r/\lambda$. Let $\mathbf R=\overline{\mathbf r}-\mathbf r_0$. The [Kelvin transform](../../../partial-differential-equation.md#kelvin-transform) correction in the first bracket is transformed using

$$
\mathbf R=\lambda^{-1}(\mathbf r-\lambda\mathbf r_0),
\qquad R=\lambda^{-1}|\mathbf r-\lambda\mathbf r_0|,
\qquad \frac{\overline r}{a}=\lambda^{-1/2}.
$$

Thus its dipole contribution is exactly

$$
\frac{1}{4\pi\sigma}\mathbf Q\cdot
\frac{\overline r}{a}\frac{\mathbf R}{R^3}
=\lambda^{3/2}\Psi(\mathbf r;\lambda\mathbf r_0).
$$

For the remaining correction use the [dipole line-integral identity](../../../calculus.md#dipole-line-integral-identity). Writing $\mathbf P_c=\mathbf r-c\mathbf r_0$ and $P_c=|\mathbf P_c|$, it is

$$
\int_0^c\frac{\mathbf r-t\mathbf r_0}{|\mathbf r-t\mathbf r_0|^3}\,dt
=\frac{c(P_c\mathbf r+r\mathbf P_c)}{rP_c(rP_c+\mathbf r\cdot\mathbf P_c)}.
$$

It can be proved by differentiating the right side with respect to $c$ and checking its zero value at $c=0$. Alternatively resolve into directions parallel and perpendicular to $\mathbf r_0=b\mathbf e$: if $\mathbf r=\rho\mathbf e_\rho+z\mathbf e$, the two integrals are $(z/r-(z-bc)/P_c)/(b\rho)$ and $(1/P_c-1/r)/b$, respectively, which combine to the displayed expression. The limiting cases follow by continuity.

Set $c=\lambda$. Then $\mathbf P_c=\lambda\mathbf R$, $P_c=\lambda R$, $\mathbf r=\lambda\overline{\mathbf r}$ and $r=\lambda\overline r$. Substitution gives

$$
\sqrt\lambda\int_0^\lambda
\frac{\mathbf r-t\mathbf r_0}{|\mathbf r-t\mathbf r_0|^3}\,dt
=\frac{R\overline{\mathbf r}+\overline r\mathbf R}
{aR(\overline rR+\overline{\mathbf r}\cdot\mathbf R)}.
$$

Dotting with $\mathbf Q/(4\pi\sigma)$ reproduces the second correction. Including the primary dipole therefore proves the [Spherical Neumann dipole images](../../../mathematics.md#spherical-neumann-dipole-images) representation,

$$
\boxed{u^-(\mathbf r)=\Psi(\mathbf r;\mathbf r_0)
+\left(\frac ra\right)^3\Psi\!\left(\mathbf r;\left(\frac ra\right)^2\mathbf r_0\right)
+\frac ra\int_0^{(r/a)^2}\Psi(\mathbf r;t\mathbf r_0)\,dt.}
$$

The upper limit is $(r/a)^2$ in the PDF; extracting the small stacked fraction as text can incorrectly invert it. The extra terms are one scaled dipole and a continuous dipole line in this parametrized [method of images](../../../mathematics.md#method-of-images). Their positions and strengths depend on the observation radius, so they should not be treated as a fixed set of independent physical sources. For an interior point $r<a$, the entire image segment satisfies $t|\mathbf r_0|\leq(r/a)^2|\mathbf r_0|<r$, so it introduces no new interior singularity. The only physical interior dipole singularity remains at $\mathbf r_0$.

## 4

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $\overline{\mathbf r}=a^2\mathbf r/r^2$ and $\widehat{\mathbf r}=\mathbf r/r$. Its Jacobian is

$$
\frac{\partial\overline r_i}{\partial r_j}
=\frac{a^2}{r^2}(\delta_{ij}-2\widehat r_i\widehat r_j).
$$

The [chain rule](../../../calculus.md#chain-rule) therefore yields

$$
\nabla_{\mathbf r}
=\frac{a^2}{r^2}
\left[\nabla_{\overline{\mathbf r}}
-2\widehat{\mathbf r}(\widehat{\mathbf r}\cdot\nabla_{\overline{\mathbf r}})\right].
$$

Taking its [cross product](../../../vector-space.md#cross-product) with $\mathbf r$ kills the radial term and proves that [spherical inversion preserves angular derivatives](../../../partial-differential-equation.md#spherical-inversion-preserves-angular-derivatives):

$$
\boxed{\mathbf r\times\nabla_{\mathbf r}
=\frac{a^2}{r^2}\mathbf r\times\nabla_{\overline{\mathbf r}}
=\overline{\mathbf r}\times\nabla_{\overline{\mathbf r}}.}
$$

This is also the invariance of the differential expression underlying the [angular momentum operator](../../../quantum-mechanics.md#angular-momentum-operator).

A scalar [spherical harmonic](../../../analysis.md#spherical-harmonic) $Y$ depends only on direction, so $Y(\widehat{\mathbf r})=Y(\widehat{\overline{\mathbf r}})$ and its gradient is tangential. Thus $\widehat{\mathbf r}\cdot\nabla_{\overline{\mathbf r}}Y=0$, and

$$
r\nabla_{\mathbf r}Y=\overline r\nabla_{\overline{\mathbf r}}Y,
\qquad \widehat{\mathbf r}=\widehat{\overline{\mathbf r}}.
$$

Each of the three normalized [vector spherical harmonic](../../../analysis.md#vector-spherical-harmonic) families is consequently unchanged as an angular basis function:

$$
\boxed{\mathbf P(\overline{\mathbf r})=\mathbf P(\mathbf r),
\qquad \mathbf B(\overline{\mathbf r})=\mathbf B(\mathbf r),
\qquad \mathbf C(\overline{\mathbf r})=\mathbf C(\mathbf r).}
$$

The normalization requires $n\geq1$ for $\mathbf B$ and $\mathbf C$; at $n=0$ the gradient vanishes and only $\mathbf P$ remains.

This substitution into the basis functions is distinct from the [pushforward of a vector field](../../../differential-geometry.md#pushforward-of-a-vector-field) of a physical vector field by inversion. Under that Jacobian map the radial vector picks up $-a^2/r^2$ and the two tangential vectors pick up $+a^2/r^2$. Likewise, the weighted [Kelvin transform](../../../partial-differential-equation.md#kelvin-transform) of a scalar includes the extra factor $a/r$. Neither operation changes the angular differential identity just proved.

## 5

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a degree-$n$ [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial), the [Euler homogeneous function theorem](../../../real-analysis.md#euler-theorem-for-homogeneous-functions) gives $\mathbf r\cdot\nabla H_n=nH_n$. On $r>0$ in three-dimensional [Euclidean space](../../../functional-analysis.md#euclidean-norm),

$$
\nabla r^s=s r^{s-2}\mathbf r,\qquad \Delta r^s=s(s+1)r^{s-2}.
$$

Apply the [product rule for the Laplacian](../../../calculus.md#product-rule-for-the-laplacian):

$$
\Delta(r^sH_n)
=r^s\Delta H_n+2s r^{s-2}\mathbf r\cdot\nabla H_n+s(s+1)r^{s-2}H_n
=r^s\Delta H_n+s(2n+s+1)r^{s-2}H_n.
$$

For $s=-(2n+1)$ the second term vanishes. Hence [homogeneous harmonic inversion](../../../analysis.md#homogeneous-harmonic-inversion) gives

$$
\boxed{\Delta\!\left(\frac{H_n}{r^{2n+1}}\right)
=\frac{\Delta H_n}{r^{2n+1}},\qquad r>0.}
$$

The nonzero factor $r^{-(2n+1)}$ proves both directions: the transformed function is [harmonic](../../../partial-differential-equation.md#harmonic-function) exactly when $\Delta H_n=0$ away from the origin. Since $\Delta H_n$ is a polynomial, vanishing on the punctured space makes it identically zero everywhere.

Equivalently, homogeneity shows that the [Kelvin transform](../../../partial-differential-equation.md#kelvin-transform) is

$$
K_aH_n(\mathbf r)=\frac arH_n\!\left(\frac{a^2}{r^2}\mathbf r\right)
=a^{2n+1}\frac{H_n(\mathbf r)}{r^{2n+1}}.
$$

It sends a [regular solid harmonic](../../../analysis.md#regular-solid-harmonic) to an [irregular solid harmonic](../../../analysis.md#irregular-solid-harmonic), exchanging the radial powers $r^n$ and $r^{-n-1}$. The origin is excluded from the harmonicity statement: for example, the $n=0$ transform $1/r$ is harmonic only away from zero and has a distributional [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) source there.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
