<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Retain only fields independent of the circle coordinate $y$, with coordinate period $2\pi r_0$. Use the [string-frame metric](../../../../../string-frame-metric.md) $g_{\mu\nu}$ and the [circle reduction of eleven-dimensional supergravity](../../../../../circle-reduction-of-eleven-dimensional-supergravity.md) ansatz

$$
ds_{11}^2=e^{-2\Phi/3}g_{\mu\nu}dx^\mu dx^\nu+e^{4\Phi/3}(dy-C_1)^2,\qquad
A_3=C_3+B_2\wedge dy.
$$

The minus sign in the fibre one-form is a convention chosen to give the usual $\widetilde F_4=dC_3-C_1\wedge H_3$ below; changing the sign of $C_1$ consistently changes no physics. The metric supplies the ten-dimensional graviton, [dilaton](../../../../../dilaton.md) and RR one-form, while the eleven-dimensional three-form supplies the [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and RR three-form. Define

$$
\eta=dy-C_1,\quad F_2=dC_1,\quad H_3=dB_2,\quad G_4=dC_3,\quad
\widetilde F_4=G_4-C_1\wedge H_3.
$$

Then $F_4^{(11)}=\widetilde F_4+H_3\wedge\eta$. In particular $d\widetilde F_4=-F_2\wedge H_3$, the reduced [Bianchi identity](../../../../../bianchi-identity.md). The field strength, not bare $dC_3$ alone, is the gauge-covariant horizontal component.

For the gravitational term, the block determinant gives

$$
\sqrt{-G}=e^{-8\Phi/3}\sqrt{-g}.
$$

A useful two-step curvature calculation first removes the overall factor $e^{-2\Phi/3}$. The intermediate metric $d\bar s^2=ds_s^2+e^{2\Phi}\eta^2$ has

$$
\bar R=R[g]-\frac14e^{2\Phi}F_{2,\mu\nu}F_2^{\mu\nu}-2\nabla^2\Phi-2(\nabla\Phi)^2,
\qquad \bar\nabla^2\Phi=\nabla^2\Phi+(\nabla\Phi)^2.
$$

The eleven-dimensional conformal-curvature identity then gives

$$
R[G]=e^{2\Phi/3}\left[\bar R+\frac{20}3\bar\nabla^2\Phi-10(\bar\nabla\Phi)^2\right].
$$

Combining the terms yields

$$
\sqrt{-G}R[G]=\sqrt{-g}\left\{
e^{-2\Phi}\left[R+\frac{14}3\nabla^2\Phi-\frac{16}3(\nabla\Phi)^2\right]
-\frac14F_{2,\mu\nu}F_2^{\mu\nu}\right\}.
$$

Integration by parts gives $\int\sqrt{-g}e^{-2\Phi}\nabla^2\Phi=2\int\sqrt{-g}e^{-2\Phi}(\nabla\Phi)^2$ modulo boundary terms. Therefore the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) produces

$$
\sqrt{-g}\left[e^{-2\Phi}(R+4(\nabla\Phi)^2)-\frac14F_{2,\mu\nu}F_2^{\mu\nu}\right].
$$

This explicitly derives both the string-frame dilaton kinetic coefficient and the RR one-form kinetic term.

Use the normalized form norm $|F_k|^2=F_{\mu_1\cdots\mu_k}F^{\mu_1\cdots\mu_k}/k!$, interpreting the printed four-form square in this convention. The horizontal and fibre pieces are orthogonal in the $\eta$ basis. Four horizontal inverse metrics contribute $e^{8\Phi/3}$ to $|\widetilde F_4|_{11}^2$. Three horizontal inverse metrics and one fibre inverse metric contribute $e^{2\Phi/3}$ to $|H_3\wedge\eta|_{11}^2$. Thus

$$
\sqrt{-G}|F_4^{(11)}|^2=\sqrt{-g}\left[|\widetilde F_4|^2+e^{-2\Phi}|H_3|^2\right].
$$

The NS-NS three-form has the same $e^{-2\Phi}$ prefactor as gravity; the RR kinetic terms do not have it in the [string frame](../../../../../string-frame-metric.md).

Finally reduce the topological term using the coordinate decomposition, which makes its signs transparent. The part of $A_3\wedge F_4^{(11)}\wedge F_4^{(11)}$ containing exactly one $dy$ is

$$
\left[B_2\wedge G_4\wedge G_4+2C_3\wedge G_4\wedge H_3\right]\wedge dy.
$$

The purely horizontal eleven-form vanishes on the ten-dimensional base. Since

$$
d(C_3\wedge B_2\wedge G_4)=B_2\wedge G_4\wedge G_4-C_3\wedge H_3\wedge G_4,
$$

integration over the base turns the bracket into $3B_2\wedge G_4\wedge G_4$, modulo the displayed exact term. The [reduction of the eleven-dimensional Chern-Simons term](../../../../../reduction-of-the-eleven-dimensional-chern-simons-term.md) therefore gives $-\tfrac12\int B_2\wedge G_4\wedge G_4$.

Absorbing the coordinate circumference into $\kappa_{10}^2=\kappa_{11}^2/(2\pi r_0)$, the complete bosonic massless [type IIA supergravity](../../../../../type-iia-supergravity.md) action in these conventions is

$$
\boxed{\begin{aligned}
S_{10}=\frac1{2\kappa_{10}^2}\Bigg\{&\int d^{10}x\sqrt{-g}\left[
e^{-2\Phi}\left(R+4(\nabla\Phi)^2-\frac12|H_3|^2\right)
-\frac12|F_2|^2-\frac12|\widetilde F_4|^2\right]\\
&-\frac12\int B_2\wedge G_4\wedge G_4\Bigg\}.
\end{aligned}}
$$

Dropping boundary terms assumes appropriate boundary conditions; nontrivial flux bundles may require patchwise potentials. Higher circle modes and higher-derivative corrections are excluded by this low-energy zero-mode reduction. No Romans-mass term arises from the ordinary ansatz.

The [M-theory origin of type IIA D-branes](../../../../../m-theory-origin-of-type-iia-d-branes.md) follows by momentum, wrapping and magnetic geometry:

| IIA object | Eleven-dimensional origin | Charge interpretation |
| --- | --- | --- |
| [D0-brane](../../../../../d0-brane.md) | Momentum along the M-circle, or its gravitational wave solution | Electric charge of the circle vector $C_1$ |
| [D2-brane](../../../../../d2-brane.md) | Unwrapped [M2-brane](../../../../../m2-brane.md) | Electric charge of $C_3$ |
| [D4-brane](../../../../../d4-brane.md) | [M5-brane](../../../../../m5-brane.md) wrapped once around the circle | Magnetic charge dual to $C_3$ |
| [D6-brane](../../../../../d6-brane.md) | [Kaluza-Klein monopole](../../../../../kaluza-klein-monopole.md) with the M-circle as its Taub–NUT fibre | Magnetic charge of $C_1$ |

An [M2-brane](../../../../../m2-brane.md) wrapped around the circle gives the [fundamental string](../../../../../fundamental-string.md), and an unwrapped [M5-brane](../../../../../m5-brane.md) gives the [NS5-brane](../../../../../ns5-brane.md). These are NS objects rather than D-branes. In physical string/Planck units, the [M-theory circle duality](../../../../../m-theory-circle-duality.md) relations are

$$
R_{11}=g_s\ell_s,\qquad\ell_p^3=g_s\ell_s^3,\qquad\ell_s^2=\alpha'.
$$

They involve the physical asymptotic radius, distinguished from the arbitrary coordinate period used in the reduction ansatz. For example, $m_{D0}=1/(g_s\ell_s)=1/R_{11}$ is one momentum quantum. With $T_{M2}=1/[(2\pi)^2\ell_p^3]$ and $T_{M5}=1/[(2\pi)^5\ell_p^6]$,

$$
T_{D2}=T_{M2},\qquad
T_{D4}=2\pi R_{11}T_{M5}=\frac1{(2\pi)^4g_s\ell_s^5},\qquad
T_{F1}=2\pi R_{11}T_{M2}=\frac1{2\pi\ell_s^2}.
$$

The [D6-brane](../../../../../d6-brane.md) is purely gravitational in eleven dimensions, rather than an elementary six-dimensional membrane; the circle-fibration magnetic charge gives its ten-dimensional interpretation.

A [D8-brane](../../../../../d8-brane.md) is the important qualification. It sources the zero-form flux of [massive type IIA supergravity](../../../../../massive-type-iia-supergravity.md) and is not obtained as an ordinary wrapped M2/M5 or Kaluza-Klein object of the undeformed circle reduction above. Its extended/generalized lifts are outside this simple dictionary. The massless-circle interpretation of the other branes is developed in [Four Lectures on M-theory](https://arxiv.org/abs/hep-th/9612121).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
