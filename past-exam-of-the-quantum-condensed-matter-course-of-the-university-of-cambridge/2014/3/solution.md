<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Diagonalization and conventions.** The spin-dependent part is $\lambda(-k_y\sigma_x+k_x\sigma_y)$. For a Hermitian [Hamiltonian](../../../hamiltonian.md) $\lambda$ is real; the supplied lower-band [spinor](../../../spinor.md) uses the convention $\lambda>0$, which will be adopted below. The squared [spin](../../../spin.md) matrix is $\lambda^2(k_x^2+k_y^2)I$. Hence the two ordered energies are

$$
E_\pm(\mathbf k)=\frac{\hbar^2(k_x^2+k_y^2+k_z^2)}{2m}\pm|\lambda|\sqrt{k_x^2+k_y^2}.
$$

In the $k_z=0$ plane, let $k=\sqrt{k_x^2+k_y^2}$ and $q_R=2m\lambda/\hbar^2>0$. Then

$$
\boxed{E_\pm(k)=\frac{\hbar^2}{2m}(k^2\pm q_Rk),\qquad q_R=\frac{2m\lambda}{\hbar^2}.}
$$

If $\lambda<0$, use $q_R=2m|\lambda|/\hbar^2$ to retain the [energy](../../../energy-split.md) ordering, and interchange the [spin](../../../spin.md) directions assigned below. This is an isotropic [Rashba effect](../../../rashba-effect.md); $q_R$ has units of inverse length, whereas $\lambda$ has units of [energy](../../../energy-split.md) times length.

**Band minima.** Define $k_R=q_R/2$ and $E_R=\hbar^2q_R^2/(8m)$. Completing the square gives

$$
E_-(k)=\frac{\hbar^2}{2m}(k-k_R)^2-E_R.
$$

Along $k_y=k_z=0$, the radial coordinate is $|k_x|$, so the lower branch has two minima:

$$
\boxed{k_x=\pm\frac{q_R}{2},\qquad E_{-,\min}=-\frac{\hbar^2q_R^2}{8m}=-E_R.}
$$

In the full plane these are points on a circle of minima $k=k_R$. Both branches meet at $k=0$, $E=0$. Their ordered [energy](../../../energy-split.md) curves contain $|k_x|$: the lower curve descends from the crossing on either side, while the upper rises. Treating them as globally labeled smooth [spin](../../../spin.md) branches without switching labels across $k_x=0$ would obscure the lower-band minima.

**Occupied regions and [Fermi contours](../../../fermi-contour.md).** At zero [temperature](../../../temperature-split.md) each spin-split [eigenstate](../../../eigenstate.md) with [energy](../../../energy-split.md) below $E_F$ is occupied. Put

$$
D=\sqrt{k_R^2+\frac{2mE_F}{\hbar^2}}.
$$

For $-E_R<E_F<0$, $0<D<k_R$. The lower-band roots are $k_R-D$ and $k_R+D$, while the upper band is entirely empty. Thus the central [disk](../../../disk-mathematics.md) $k<k_R-D$ is **unoccupied**, the [annulus](../../../annulus-mathematics.md) $k_R-D<k<k_R+D$ is **singly occupied**, and the exterior is **unoccupied**. Both Fermi circles belong to the lower band; there is no doubly occupied region.

At $E_F=0$, the lower band is occupied for $0<k<2k_R=q_R$, giving a **singly occupied [disk](../../../disk-mathematics.md)** with outer Fermi circle at $q_R$. The two bands also meet the [Fermi energy](../../../fermi-energy.md) at the origin. That isolated degenerate point is not a finite doubly occupied [disk](../../../disk-mathematics.md), and occupation exactly at the [Fermi energy](../../../fermi-energy.md) is a boundary convention of zero area. Outside the outer circle the states are empty.

For $E_F>0$, $D>k_R$. The lower branch has outer radius $k_-=D+k_R$, while the upper branch has inner radius $k_+=D-k_R$. The [disk](../../../disk-mathematics.md) $k<k_+$ is **doubly occupied**, with one state in each band at every [momentum](../../../momentum-split.md). The [annulus](../../../annulus-mathematics.md) $k_+<k<k_-$ is **singly occupied**, in the lower band only, and the exterior is **unoccupied**. These are the [Fermi contours of an isotropic Rashba band](../../../fermi-contours-of-an-isotropic-rashba-band.md); double occupancy here refers to two orthogonal [spinor](../../../spinor.md) states at the same [momentum](../../../momentum-split.md), not two [electrons](../../../electron.md) occupying one identical quantum state.

<a id="3/image-rashba-dispersion-and-occupied-momentum-regions-below-at-and-above-the-band-crossing"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014-rashba-occupations.png)

**[Figure 3](#3/image-rashba-dispersion-and-occupied-momentum-regions-below-at-and-above-the-band-crossing). Rashba dispersion and occupied momentum regions below, at and above the band crossing**.

**Inferring the splitting.** Above the crossing, the two positive radii differ by $2k_R=q_R$:

$$
\boxed{q_R=k_1-k_2=(0.11-0.01)\,\mathrm{\mathring A^{-1}}=0.10\,\mathrm{\mathring A^{-1}}=1.0\times10^9\,\mathrm{m^{-1}}.}
$$

The minimum radius is therefore $k_R=0.05\,\mathrm{\mathring A^{-1}}$. It is the difference of the measured radii that is required for $E_F>0$; below the crossing the two lower-band radii instead add to $q_R$.

**Spinors and [spin](../../../spin.md) direction.** Write $a=(k_y+ik_x)/k$, which has $|a|=1$ for $k>0$. An orthogonal normalized partner to the supplied lower-band state is

$$
\boxed{u_+(\mathbf k)=\frac1{\sqrt2}\begin{pmatrix}-a\\1\end{pmatrix}=\frac1{\sqrt2}\begin{pmatrix}-(k_y+ik_x)/k\\1\end{pmatrix}.}
$$

Indeed $u_-^\dagger u_+=(-|a|^2+1)/2=0$. Direct multiplication by the [spin](../../../spin.md) matrix gives [eigenvalues](../../../eigenvalue.md) $-\lambda k$ and $+\lambda k$ for $u_-$ and $u_+$, respectively, so [orthogonality](../../../orthogonal-vectors.md) has selected the other band rather than merely another arbitrary [spin](../../../spin.md) [basis](../../../basis.md).

For a normalized [spinor](../../../spinor.md) $(\alpha,\beta)^T$, the Pauli expectation values are $(2\operatorname{Re}(\alpha^*\beta),2\operatorname{Im}(\alpha^*\beta),|\alpha|^2-|\beta|^2)$. Consequently the [Rashba spin texture](../../../rashba-spin-texture.md) is

$$
\boxed{\langle\mathbf S\rangle_- =\frac\hbar2\left(\frac{k_y}{k},-\frac{k_x}{k},0\right),\qquad \langle\mathbf S\rangle_+ =\frac\hbar2\left(-\frac{k_y}{k},\frac{k_x}{k},0\right).}
$$

The [spin](../../../spin.md) lies in the plane and is perpendicular to [momentum](../../../momentum-split.md). On the outer circle $k_1$, which belongs to $E_-$, it points clockwise as viewed from $+z$; at $\mathbf k=(k_1,0)$ it points along $-y$. On the inner circle $k_2$, belonging to $E_+$, it points counterclockwise; at $\mathbf k=(k_2,0)$ it points along $+y$. Opposite momenta have opposite spins, consistent with [time-reversal symmetry](../../../t-symmetry.md). At the origin the eigenstates are degenerate and no unique [spin](../../../spin.md) orientation is defined.

<a id="3/image-opposite-tangential-spin-textures-on-the-outer-lower-band-and-inner-upper-band-fermi-circles"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014-rashba-spin-texture.png)

**[Figure 4](#3/image-opposite-tangential-spin-textures-on-the-outer-lower-band-and-inner-upper-band-fermi-circles). Opposite tangential spin textures on the outer lower-band and inner upper-band Fermi circles**.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2014](../../2014-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
