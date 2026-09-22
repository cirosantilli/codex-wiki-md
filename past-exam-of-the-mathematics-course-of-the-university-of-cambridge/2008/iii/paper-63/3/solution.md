<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $I^{ij}(t)=\int T^{00}(t,\mathbf x)x^ix^j\,d^3x$, using spatial indices $i,j$. [Stress-energy conservation](../../../../../stress-energy-conservation.md), symmetry of the [stress-energy tensor](../../../../../stress-energy-tensor.md) and [integration by parts](../../../../../integration-by-parts.md) give

$$
\dot I^{ij}=-\int\partial_kT^{0k}x^ix^j\,d^3x
=\int(T^{0i}x^j+T^{0j}x^i)\,d^3x,
$$

and a second derivative gives

$$
\ddot I^{ij}=-\int(\partial_kT^{ik}x^j+\partial_kT^{jk}x^i)\,d^3x
=\int(T^{ij}+T^{ji})\,d^3x.
$$

All boundary terms vanish by [compact support](../../../../../compact-support.md). This proves the [stress-energy quadrupole identity](../../../../../stress-energy-quadrupole-identity.md),

$$
\boxed{\int T^{ij}\,d^3x=\frac12\ddot I^{ij}.}
$$

The support is understood to remain bounded over the time interval used for differentiating these integrals.

For the radiation calculation set $c=1$, write $g_{ab}=\eta_{ab}+h_{ab}$ and use the [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$ in [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md). With the curvature and field-equation signs in this paper, the linear equation is

$$
\Box\bar h_{ab}=-16\pi GT_{ab},\qquad \Box=\partial_t^2-\nabla^2.
$$

The retarded solution with no incoming radiation is consequently

$$
\bar h_{ab}(t,\mathbf x)=-4G\int
\frac{T_{ab}(t-|\mathbf x-\mathbf x'|,\mathbf x')}
{|\mathbf x-\mathbf x'|}\,d^3x'.
$$

Let $r=|\mathbf x|$ be the distance from the source's [centre of mass](../../../../../center-of-mass.md), and let $d$ be its size. In the [radiation zone](../../../../../radiation-zone.md), $r\gg d$. The leading [multipole expansion](../../../../../electric-multipole-expansion.md) additionally assumes slow internal motion, or $d$ small compared with the radiation wavelength. These assumptions allow $|\mathbf x-\mathbf x'|\simeq r$ in the denominator and the common retarded time $u=t-r$ at leading quadrupole order. Thus

$$
\bar h_{ij}\simeq-\frac{4G}{r}\int T_{ij}(u,\mathbf x')\,d^3x'
=-\frac{2G}{r}\ddot I_{ij}(u).
$$

Define the trace-free [mass quadrupole moment](../../../../../mass-quadrupole-moment.md) by

$$
Q^{ij}=I^{ij}-\frac13\delta^{ij}I^{kk}
=\int T^{00}\left(x^ix^j-\frac13\delta^{ij}|\mathbf x|^2\right)d^3x.
$$

To make the requested normalization explicit, write the trace-free spatial metric coefficient as $h_{ij}^{\mathrm{TF}}=-2E_{ij}$. Trace reversal only adds a spatial trace, so the preceding equations give the [far-zone quadrupole strain](../../../../../far-zone-quadrupole-strain.md) coefficient

$$
\boxed{E^{ij}(t,\mathbf x)=\frac{G}{r}\ddot Q^{ij}(t-r).}
$$

The supplied scan does not contain the referenced perturbation handout. The definition above fixes the normalization of $E$ directly. If $E$ denotes the physical [transverse-traceless tensor](../../../../../transverse-traceless-tensor.md) in that handout, the right-hand side is also to be transversely projected for the observation direction. Trace-free alone does not imply transverse. With $\mathbf n=\mathbf x/r$, put

$$
P_{ij}=\delta_{ij}-n_in_j,\qquad
\Lambda_{ij,kl}=P_{i(k}P_{l)j}-\frac12P_{ij}P_{kl}.
$$

The [transverse-traceless projector](../../../../../transverse-traceless-projector.md) gives $E^{\mathrm{TT}}_{ij}=\Lambda_{ij,kl}E_{kl}$ and the physical spatial strain is $H^{\mathrm{TT}}_{ij}=2E^{\mathrm{TT}}_{ij}$. This also states the result without relying on omitted handout notation. The retarded construction and direction-dependent transverse projection are described in [Carroll's general relativity lectures](https://ned.ipac.caltech.edu/level5/March01/Carroll3/Carroll6.html), with the appropriate changes of metric-sign convention.

For the equal-mass [binary star](../../../../../binary-star.md), its [centre of mass](../../../../../center-of-mass.md) is at the origin and the separation is $2R$. The gravitational force on either star is $Gm^2/(2R)^2$, while its centripetal force is $mR\omega^2$. Hence

$$
\boxed{\omega^2=\frac{Gm}{4R^3},\qquad \theta(t)=\omega t+\theta_0.}
$$

At leading Newtonian order, $T^{00}$ is the sum of the two point-mass densities. Its moments are

$$
I^{ij}=2mR^2
\begin{pmatrix}
\cos^2\theta&\sin\theta\cos\theta&0\\
\sin\theta\cos\theta&\sin^2\theta&0\\
0&0&0
\end{pmatrix},
\qquad I^{kk}=2mR^2,
$$

so the trace-free [mass quadrupole moment](../../../../../mass-quadrupole-moment.md) is

$$
Q^{ij}=mR^2
\begin{pmatrix}
\cos2\theta+\frac13&\sin2\theta&0\\
\sin2\theta&\frac13-\cos2\theta&0\\
0&0&-\frac23
\end{pmatrix}.
$$

The Newtonian bound system is treated in the usual leading weak-field quadrupole approximation; an exactly conserved effective source also includes the interaction stresses. Accelerated point-mass dust alone would not satisfy the conservation hypothesis.

Differentiating twice and evaluating at $u=t-r$ gives

$$
\boxed{E^{ij}=-\frac{4GmR^2\omega^2}{r}
\begin{pmatrix}
\cos2\theta(u)&\sin2\theta(u)&0\\
\sin2\theta(u)&-\cos2\theta(u)&0\\
0&0&0
\end{pmatrix}.}
$$

For an observer on the $z$ axis this is already transverse and traceless. Its alternating [plus polarization](../../../../../plus-polarization.md) and [cross polarization](../../../../../cross-polarization.md) have a phase difference of $\pi/2$, giving circularly polarized [gravitational radiation](../../../../../gravitational-wave.md) at twice the orbital frequency. The amplitude decays as $1/r$, as expected for outgoing radiation in three spatial dimensions.

More generally take the line of sight in the $xz$ plane at inclination $\iota$ to the orbital angular-momentum axis. In the transverse basis $\mathbf e_\theta=(\cos\iota,0,-\sin\iota)$, $\mathbf e_\phi=(0,1,0)$, define $A=4GmR^2\omega^2/r$. Projection gives the physical [gravitational wave polarizations](../../../../../gravitational-wave-polarization.md)

$$
h_+=-A(1+\cos^2\iota)\cos2\theta(u),
\qquad h_\times=-2A\cos\iota\sin2\theta(u).
$$

Thus a generic view is elliptically polarized, the face-on view is circularly polarized and the edge-on view is linearly polarized. This is [circular-binary quadrupole radiation](../../../../../circular-binary-quadrupole-radiation.md); an overall sign or transverse-axis rotation only changes the polarization convention.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
