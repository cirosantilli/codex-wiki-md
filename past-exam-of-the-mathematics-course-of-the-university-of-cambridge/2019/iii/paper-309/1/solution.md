<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The outgoing solution obtained from the [retarded fundamental solution](../../../../../retarded-fundamental-solution.md) of the [wave equation](../../../../../wave-equation-split.md) is

$$
h_{ab}(t,\mathbf x)=4\int
\frac{T_{ab}-\tfrac12\eta_{ab}T}
{|\mathbf x-\mathbf x'|}
\left(t-|\mathbf x-\mathbf x'|,\mathbf x'\right)d^3x'.
$$

In the [radiation zone](../../../../../radiation-zone.md), put $r=|\mathbf x|$, $\mathbf n=\mathbf x/r$, and retain the leading $1/r$ term at [retarded time](../../../../../retarded-time.md) $u=t-r$. The trace term disappears after applying the [transverse-traceless projector](../../../../../transverse-traceless-projector.md)

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

Twice using [stress-energy conservation](../../../../../stress-energy-conservation.md), $\partial_aT^{ab}=0$, and integrating by parts gives

$$
\frac{d^2}{du^2}\int T_{00}x_kx_l\,d^3x
=2\int T_{kl}\,d^3x.
$$

The projector removes the trace, so in terms of the [mass quadrupole moment](../../../../../mass-quadrupole-moment.md)

$$
Q_{kl}=\int\rho
\left(x_kx_l-\frac13\delta_{kl}|\mathbf x|^2\right)d^3x
$$

the far field is

$$
\boxed{h^{\rm TT}_{ij}=\frac2r\Lambda_{ij,kl}\ddot Q_{kl}(u)}.
$$

The [gravitational-wave energy flux](../../../../../gravitational-wave-energy-flux.md) is

$$
\frac{dP}{d\Omega}
=\frac{r^2}{32\pi}
\left\langle\dot h^{\rm TT}_{ij}\dot h^{\rm TT}_{ij}\right\rangle.
$$

For a trace-free symmetric tensor $A_{ij}$, the [isotropic tensor integral](../../../../../isotropic-tensor-integral.md) over the observation direction gives

$$
\int \Lambda_{ij,kl}A_{kl}\Lambda_{ij,mn}A_{mn}\,d\Omega
=\frac{8\pi}{5}A_{ij}A_{ij}.
$$

Consequently the standard [quadrupole formula](../../../../../quadrupole-formula.md), in the units $G=c=1$ used by the paper, is

$$
\boxed{P=\frac15\left\langle\dddot Q_{ij}\dddot Q_{ij}\right\rangle}.
$$

Thus the printed coefficient $4\pi/5$ is inconsistent with the stated definition of $Q_{ij}$ and the standard wave-energy normalization; it appears to be a typographical error.

For the planet, choose its [circular orbit](../../../../../circular-orbit.md) in the $xy$-plane and write $\omega=2\pi/\tau$. With the star treated as fixed,

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

For two bodies of comparable mass, $M$ is replaced by the [reduced mass](../../../../../reduced-mass.md) and $R$ by their separation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 309](../../paper-309-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
