<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Remove the constant trace from the [second mass moment tensor](../../../../../../../second-mass-moment-tensor.md) to obtain the [mass quadrupole moment](../../../../../../../mass-quadrupole-moment.md) $Q_{ij}=I_{ij}-\delta_{ij}I_{kk}/3$. Since $I_{kk}$ is constant, $\dddot Q_{ij}=\dddot I_{ij}$. In units $G=c=1$, the [quadrupole formula](../../../../../../../quadrupole-formula.md) gives

$$
\langle P\rangle=\frac15\left\langle\dddot Q_{ij}\dddot Q_{ij}\right\rangle.
$$

Its normalization can also be seen from the [gravitational-wave energy flux](../../../../../../../gravitational-wave-energy-flux.md): $h^{\mathrm{TT}}_{ij}=2\Lambda_{ij,kl}\ddot Q_{kl}/r$, where $\Lambda$ is the [transverse-traceless projector](../../../../../../../transverse-traceless-projector.md). With $S_{ij}=\dddot Q_{ij}$ and $P_{ij}=\delta_{ij}-n_i n_j$, the projection is $S^{\mathrm{TT}}_{ij}=P_{ik}P_{jl}S_{kl}-P_{ij}P_{kl}S_{kl}/2$. For a symmetric trace-free $S$,

$$
S^{\mathrm{TT}}_{ij}S^{\mathrm{TT}}_{ij}
=S_{ij}S_{ij}-2n_iS_{ij}S_{jk}n_k+\frac12(n_iS_{ij}n_j)^2.
$$

The [isotropic tensor integrals](../../../../../../../isotropic-tensor-integral.md) $\int n_i n_j\,d\Omega=4\pi\delta_{ij}/3$ and $\int n_i n_j n_k n_l\,d\Omega=4\pi(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk})/15$ therefore give $\int |S^{\mathrm{TT}}|^2d\Omega=8\pi S_{ij}S_{ij}/5$. Integrating the flux yields $\langle P\rangle=(8\pi)^{-1}\int\langle |S^{\mathrm{TT}}|^2\rangle d\Omega=\langle S_{ij}S_{ij}\rangle/5$, as above.

Now differentiate the components from part (i). With $\Delta=I_1-I_2$,

$$
\begin{aligned}
\dddot I_{11}&=4\Delta\Omega^3\sin(2\Omega t),&
\dddot I_{22}&=-4\Delta\Omega^3\sin(2\Omega t),\\
\dddot I_{12}=\dddot I_{21}&=-4\Delta\Omega^3\cos(2\Omega t),&
\dddot I_{33}&=0.
\end{aligned}
$$

The off-diagonal component occurs twice in the contraction. Thus

$$
\dddot I_{ij}\dddot I_{ij}
=32\Delta^2\Omega^6[\sin^2(2\Omega t)+\cos^2(2\Omega t)]
=32\Delta^2\Omega^6.
$$

It is already time independent, so averaging gives

$$
\boxed{\langle P\rangle=\frac{32}{5}\Omega^6(I_1-I_2)^2.}
$$

This is the leading [gravitational radiation from a rotating triaxial body](../../../../../../../gravitational-radiation-from-a-rotating-triaxial-body.md); restoring units multiplies it by $G/c^5$. The source is treated as rotating uniformly over an averaging interval, with radiation reaction negligible at this order.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
