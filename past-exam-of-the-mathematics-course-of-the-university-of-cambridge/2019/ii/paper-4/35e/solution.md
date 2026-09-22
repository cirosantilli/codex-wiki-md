<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

The [source-free Maxwell equations in a linear medium](../../../../../source-free-maxwell-equations-in-a-linear-medium.md) are

$$
\boxed{
\nabla\mathbin{\cdot}\mathbf D=0,\qquad
\nabla\mathbin{\cdot}\mathbf B=0,\qquad
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t},
\qquad
\nabla\times\mathbf H=\frac{\partial\mathbf D}{\partial t}.}
$$

Here the [constitutive relations](../../../../../constitutive-relations.md) are $\mathbf D=\varepsilon\mathbf E$ and $\mathbf B=\mu\mathbf H$.

Substitution of the sinusoidal plane waves into the two divergence equations gives the [transversality of an electromagnetic plane wave](../../../../../transversality-of-an-electromagnetic-plane-wave.md),

$$
\mathbf k\mathbin{\cdot}\mathbf E_0=0,
\qquad
\mathbf k\mathbin{\cdot}\mathbf B_0=0.
$$

[Faraday's law](../../../../../faraday-s-law-of-induction.md) and the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) give, respectively,

$$
\mathbf k\times\mathbf E_0=\omega\mathbf B_0,
\qquad
\mathbf k\times\mathbf B_0=-\mu\varepsilon\omega\mathbf E_0.
$$

Taking $\mathbf k\times$ the first equation and using transversality yields

$$
-k^2\mathbf E_0
=-\mu\varepsilon\omega^2\mathbf E_0.
$$

Thus a nonzero [plane electromagnetic wave in a linear medium](../../../../../plane-electromagnetic-wave-in-a-linear-medium.md) must satisfy

$$
\boxed{
k^2=\mu\varepsilon\omega^2,\qquad
\mathbf B_0=\frac{\mathbf k\times\mathbf E_0}{\omega},\qquad
v_{\rm ph}=\frac{\omega}{k}=\frac1{\sqrt{\mu\varepsilon}}.}
$$

In particular, $\mathbf E_0$, $\mathbf B_0$, and $\mathbf k$ are mutually orthogonal, with $|\mathbf B_0|=\sqrt{\mu\varepsilon}\,|\mathbf E_0|$.

Take the interface to be $x=0$ and the plane of incidence to be the $xy$-plane. The incident, reflected, and transmitted wavevectors may be written

$$
\begin{aligned}
\mathbf k_I&=k_-(\cos\theta_I,\sin\theta_I,0),\\
\mathbf k_R&=k_-(-\cos\theta_R,\sin\theta_R,0),\\
\mathbf k_T&=k_+(\cos\theta_T,\sin\theta_T,0).
\end{aligned}
$$

The [phase matching at a planar wave interface](../../../../../phase-matching-at-a-planar-wave-interface.md) requires one common angular frequency and one common tangential wavevector:

$$
k_-\sin\theta_I
=k_-\sin\theta_R
=k_+\sin\theta_T.
$$

Since $k_\pm=\omega\sqrt{\varepsilon_\pm\mu}
=n_\pm\omega/c$, this gives the [Snell law for electromagnetic waves](../../../../../snell-law-for-electromagnetic-waves.md),

$$
\boxed{\theta_R=\theta_I,\qquad
n_-\sin\theta_I=n_+\sin\theta_T.}
$$

For the final polarization, take the signed electric amplitudes along $\widehat{\mathbf z}$. The [dielectric-interface boundary conditions](../../../../../dielectric-interface-boundary-conditions.md) require continuity of tangential $\mathbf E$ and $\mathbf H$. Since

$$
\mathbf H=\frac{\mathbf k\times\mathbf E}{\mu\omega},
$$

their $z$- and $y$-components give

$$
E_I+E_R=E_T,
$$

and

$$
k_-\cos\theta_I(E_I-E_R)
=k_+\cos\theta_T E_T.
$$

Eliminating $E_I$ yields

$$
\frac{E_R}{E_T}
=\frac12\left(
1-\frac{k_+\cos\theta_T}{k_-\cos\theta_I}
\right).
$$

Using $\theta_R=\theta_I$ and Snell's law,

$$
\frac{k_+\cos\theta_T}{k_-\cos\theta_I}
=\frac{\sin\theta_R\cos\theta_T}
{\sin\theta_T\cos\theta_R}
=\frac{\tan\theta_R}{\tan\theta_T}.
$$

Therefore the [reflected-to-transmitted transverse-electric amplitude ratio](../../../../../reflected-to-transmitted-transverse-electric-amplitude-ratio.md) is

$$
\boxed{
\frac{|\mathbf E_R|}{|\mathbf E_T|}
=\frac12\left(
1-\frac{\tan\theta_R}{\tan\theta_T}
\right),}
$$

with the polarization directions chosen so that the displayed signed factor is nonnegative; otherwise its absolute value gives the magnitude ratio.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
