<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use geometrized units $G=c=1$ and signature $(-,+,+,+)$. The original PDF starts with the [d'Alembert operator](../../../../../../d-alembert-operator.md) $\Box\bar h_{\mu\nu}=-16\pi T_{\mu\nu}$; the local TeX incorrectly transcribes its derivative indices. The harmonic condition is the [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md).

Choose the retarded solution, excluding an incoming homogeneous wave. For a spatially localized source, the [Linearized Einstein equations](../../../../../../linearized-einstein-equations.md) give

$$
\bar h_{\mu\nu}(t,\mathbf x)
=4\int\frac{T_{\mu\nu}(t-|\mathbf x-\mathbf y|,\mathbf y)}{|\mathbf x-\mathbf y|}\,d^3y.
$$

Let the source size be $D$ and the characteristic angular frequency be $\omega$. Assume the [weak-field approximation](../../../../../../weak-field-approximation.md), nonrelativistic source velocities, and $D\ll\omega^{-1}\ll r$ for a radiative far-zone measurement. Then $|\mathbf x-\mathbf y|=r-\mathbf n\cdot\mathbf y+O(D^2/r)$. At leading order in $D/r$ and $\omega D$, one may replace the denominator by $r$ and the retarded time throughout the source by $t-r$, obtaining

$$
\bar h_{ij}(t,\mathbf x)\simeq\frac4r\int T_{ij}(t-r,\mathbf y)\,d^3y.
$$

To identify this integral, use [stress-energy conservation](../../../../../../stress-energy-conservation.md) $\partial_\mu T^{\mu\nu}=0$ for a symmetric source tensor. Compact support or sufficient decay permits [integration by parts](../../../../../../integration-by-parts.md) with no boundary flux. Because $T^{00}=T_{00}$ in this signature, the [second mass moment tensor](../../../../../../second-mass-moment-tensor.md) satisfies

$$
\begin{aligned}
\dot I_{ij}
&=-\int\partial_kT^{k0}\,y_i y_j\,d^3y
=\int(T^{i0}y_j+T^{j0}y_i)\,d^3y,\\
\ddot I_{ij}
&=-\int\bigl(\partial_kT^{ki}\,y_j+\partial_kT^{kj}\,y_i\bigr)\,d^3y
=2\int T^{ij}\,d^3y.
\end{aligned}
$$

Spatial indices are raised with $\delta_{ij}$, so $T^{ij}=T_{ij}$. Substitution gives the [retarded quadrupole field](../../../../../../retarded-quadrupole-field.md):

$$
\boxed{\bar h_{ij}(t,\mathbf x)\simeq\frac2r\ddot I_{ij}(t-r).}
$$

The assumptions are an isolated conserved source, retarded boundary conditions, weak gravity, a source small compared with the wavelength, and observation far from it. The physical radiative field follows by the [transverse-traceless projector](../../../../../../transverse-traceless-projector.md) applied to this [trace-reversed metric perturbation](../../../../../../trace-reversed-metric-perturbation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
