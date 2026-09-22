<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

There is a genuine periodicity mismatch in the source. Write $x_s=sb+u_s$. The intended [periodic displacements in a harmonic chain](../../../../../periodic-displacements-in-a-harmonic-chain.md) satisfy $u_N=u_0$, equivalently $x_N=x_0+Nb$ for unwrapped positions. The printed $x_N=x_0$ instead makes the potential $\frac12m\lambda^2\sum_s(x_{s+1}-x_s)^2+\frac12Nm\lambda^2b^2$, with equilibrium at equal positions, not $x_s=sb$. The following lattice derivation uses periodic displacements, as required by the requested position operator.

Put $k_r=2\pi r/(Nb)$, $r=0,\ldots,N-1$, and [Fourier transform](../../../../../fourier-transform.md) the displacements and momenta with normalization $N^{-1/2}$. The spring quadratic form is diagonal, with factor $|e^{ik_rb}-1|^2=4\sin^2(k_rb/2)$. Thus each nonzero mode is a [harmonic oscillator](../../../../../simple-harmonic-motion.md) with

$$
\boxed{\omega_r=2\lambda|\sin(k_rb/2)|.}
$$

Creation and annihilation operators obey $[a_r,a_{r'}^\dagger]=\delta_{rr'}$. Inverting the oscillator-coordinate expansion gives

$$
\boxed{x_s=sb+\sqrt{\frac{\hbar}{2mN}}\sum_{r\ne0}\frac{a_re^{ik_rsb}+a_r^\dagger e^{-ik_rsb}}{\sqrt{\omega_r}}.}
$$

The conjugate momentum is $p_s=-i\sqrt{m\hbar/(2N)}\sum_{r\ne0}\sqrt{\omega_r}(a_re^{ik_rsb}-a_r^\dagger e^{-ik_rsb})$. Fourier orthogonality diagonalizes the [Hamiltonian](../../../../../hamiltonian.md) as $\sum_{r\ne0}\hbar\omega_r(a_r^\dagger a_r+1/2)$. The normalized oscillator vacuum is annihilated by every $a_r$; applying creation operators gives [number states](../../../../../number-state.md), each added [phonon](../../../../../phonon.md) contributing $\hbar\omega_r$. The omitted zero mode is a free centre-of-mass coordinate, which must be fixed or treated separately rather than assigned an oscillator vacuum. Accordingly the reduced displacement commutator is $[u_s,p_t]=i\hbar(\delta_{st}-1/N)$.

For $iq u_s$, separate creation and annihilation parts. Their commutator is a scalar, so the supplied [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md) and vacuum expectations give

$$
\langle0|e^{iqu_s}|0\rangle=e^{-W(q)},\qquad W(q)=\frac{q^2\hbar}{4mN}\sum_{r\ne0}\frac1{\omega_r}.
$$

Summing the geometric lattice phases yields

$$
\boxed{M=e^{-W(q)}e^{iqb(N-1)/2}\frac{\sin(Nqb/2)}{\sin(qb/2)},\qquad |M|^2=e^{-2W(q)}\left[\frac{\sin(Nqb/2)}{\sin(qb/2)}\right]^2.}
$$

The ratio is interpreted by continuity at its removable singularities. The interference factor has its maximum $N^2$ at $q=2\pi n/b$, where all lattice phases coincide. The source's Fourier-sum hint should read $r\equiv0\pmod N$, rather than $r=Nb$.

The claim about the full matrix element also needs qualification: its [Debye–Waller factor](../../../../../debye-waller-factor.md) envelope varies with $q$. The absolute global maximum is $|M(0)|^2=N^2$; at nonzero reciprocal-lattice points the value is $N^2e^{-2W(2\pi n/b)}<N^2$. Moreover the derivative of the envelope there is nonzero, whereas that of the interference factor is zero, so those points are not exact local maxima of the full finite-chain intensity. **The reciprocal-lattice condition maximizes the interference factor**, which is the usual constructive-scattering interpretation of the requested result.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
