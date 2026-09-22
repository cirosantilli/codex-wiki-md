<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

The linear acoustic momentum and [continuity](../../../../../continuous-function.md) equations are $\rho u_t=-p_x$ and $p_t=-\rho c^2u_x$. For a right-moving [plane wave](../../../../../plane-wave.md) depending on $x-ct$, integration gives $\boxed{p=\rho c\,u}$, with zero perturbation constants. For a left-moving wave the sign is reversed. The factor $Z=\rho c$ is the [acoustic impedance](../../../../../acoustic-impedance.md). Proportionality applies to a traveling wave; a superposition of opposite directions generally has no single such constant.

Use time dependence $e^{-i\omega t}$ and set $Z_j=\rho_jc_j$. In the outer regions write pressures $I e^{ik_0x}+R e^{-ik_0x}$ and $T I e^{ik_0x}$, taking $I=1$ for convenience. The corresponding velocities are $(e^{ik_0x}-R e^{-ik_0x})/Z_0$ and $Te^{ik_0x}/Z_0$. Pressure and normal velocity are continuous at both layer boundaries. Within the cooled layer a decomposition into right and left waves gives, with $\delta=k_1L$,

$$
\begin{pmatrix}p(L)\\u(L)\end{pmatrix}=
\begin{pmatrix}\cos\delta&iZ_1\sin\delta\\ i\sin\delta/Z_1&\cos\delta\end{pmatrix}
\begin{pmatrix}p(0)\\u(0)\end{pmatrix}.
$$

This matrix follows by writing $p=Ae^{ik_1x}+Be^{-ik_1x}$ and $Z_1u=Ae^{ik_1x}-Be^{-ik_1x}$. Applying its inverse and using $p(0)+Z_0u(0)=2$ eliminates $R$, giving

$$
T=\frac{e^{-ik_0L}}{\cos\delta-\frac i2(\lambda+\lambda^{-1})\sin\delta},\qquad \lambda=Z_1/Z_0.
$$

Consequently

$$
\boxed{|T|=\left[\cos^2(k_1L)+\frac14(\lambda+\lambda^{-1})^2\sin^2(k_1L)\right]^{-1/2}.}
$$

For $\lambda\gg1$, transmission is weak except near $k_1L=n\pi$, where $|T|=1$. The cooled layer acts as a resonant filter: an [integer](../../../../../integer.md) number of half-wavelengths fits within it at each [resonance](../../../../../resonance.md). The half-power width in $\delta$ is asymptotically $2/\lambda$ on either side. Since the two outer impedances agree, the transmitted power fraction is $|T|^2$.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
