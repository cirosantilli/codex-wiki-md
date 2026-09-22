<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

Label the two displacements in cell $n$ by $u_n,v_n$, with cell length $2a$. Choose the $K$ spring within a cell and the $G$ spring between cells. The equations are

$$
m\ddot u_n=-(K+G)u_n+Kv_n+Gv_{n-1},\qquad
m\ddot v_n=-(K+G)v_n+Ku_n+Gu_{n+1}.
$$

A [Bloch wave](../../../../../bloch-state.md) $(u_n,v_n)=(u,v)e^{i(2aqn-\omega t)}$ gives a two-by-two [eigenvalue](../../../../../eigenvalue.md) problem, whose determinant is

$$
(K+G-m\omega^2)^2-(K+Ge^{-2iaq})(K+Ge^{2iaq})=0.
$$

Thus the [alternating-spring chain dispersion relation](../../../../../alternating-spring-chain-dispersion-relation.md) is

$$
\boxed{\omega_\pm^2(q)=\frac{K+G\pm\sqrt{K^2+G^2+2KG\cos(2aq)}}m.}
$$

Periodic boundaries require $e^{2iaqN}=1$, so $q=\pi j/(Na)$ modulo $\pi/a$. There are $N$ distinct wavenumbers in the [Brillouin zone](../../../../../brillouin-zone.md) $-\pi/(2a)\leq q<\pi/(2a)$ and two branches, accounting for $2N$ modes. The minus branch is acoustic, with zero frequency and in-phase motion at the centre; the plus branch is optical, with opposite cell displacements.

Expanding the square root near zero gives

$$
\boxed{\omega_-(q)\sim a\sqrt{\frac{2KG}{m(K+G)}}|q|,\qquad
\omega_+(q)\sim\sqrt{\frac{2(K+G)}m}
\left[1-\frac{KG a^2q^2}{2(K+G)^2}\right].}
$$

At the zone boundary the square root is $K-G$, so the acoustic maximum is $\sqrt{2G/m}$ and the optical minimum is $\sqrt{2K/m}$. The frequency gap is therefore

$$
\boxed{\Delta\omega=\sqrt{2K/m}-\sqrt{2G/m}.}
$$

Quantizing each harmonic mode gives [phonons](../../../../../phonon.md), bosonic excitations of energy $\hbar\omega_\pm(q)$ and crystal momentum $\hbar q$ defined modulo a reciprocal lattice vector. Their [group velocity](../../../../../group-velocity.md) is $d\omega/dq$; acoustic [phonons](../../../../../phonon.md) carry long-wavelength sound, while optical [phonons](../../../../../phonon.md) have a nonzero centre frequency. There is one longitudinal polarization per branch here, and [phonon](../../../../../phonon.md) number is not conserved in thermal equilibrium.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
