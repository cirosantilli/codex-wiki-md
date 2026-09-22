<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one bosonic mode, define the [unnormalized bosonic coherent state](../../../../../unnormalized-bosonic-coherent-state.md) $|z\rangle=e^{z a^\dagger}|0\rangle$. The [commutator](../../../../../commutator.md) $[a,a^\dagger]=1$ gives $a|z\rangle=z|z\rangle$ and $\langle z'|z\rangle=e^{\bar z'z}$. The normalized state is $e^{-|z|^2/2}|z\rangle$; it is not orthogonal to a different [coherent state](../../../../../coherent-state.md). The [coherent-state resolution of identity](../../../../../coherent-state-resolution-of-identity.md) follows from Gaussian moments,

$$
\int\frac{d^2z}{\pi}e^{-|z|^2}z^n\bar z^m=n!\delta_{nm},\qquad \boxed{\mathbf1=\int\frac{d^2z}{\pi}e^{-|z|^2}|z\rangle\langle z|.}
$$

For many modes take products of these states and measures. The complex amplitudes have the natural scale of square root occupation; [coherent states](../../../../../coherent-state.md) turn normal-ordered [matrix elements](../../../../../matrix-element.md) into classical symbols without replacing the quantum [trace](../../../../../matrix-trace.md) by a single classical configuration.

For [fermions](../../../../../fermion.md), $\{c_i,c_j^\dagger\}=\delta_{ij}$ and a nilpotent [annihilation operator](../../../../../annihilation-operator.md) cannot have an arbitrary nonzero ordinary complex [eigenvalue](../../../../../eigenvalue.md). Introduce independent [Grassmann variables](../../../../../grassmann-variable.md) $\eta_i,\bar\eta_i$, anticommuting among themselves and with the fermionic operators, and define $|\eta\rangle=\exp(-\sum_i\eta_i c_i^\dagger)|0\rangle$. Then $c_i|\eta\rangle=\eta_i|\eta\rangle$ and $\langle\bar\eta'|\eta\rangle=e^{\sum_i\bar\eta_i'\eta_i}$. With an ordered [Berezin integral](../../../../../berezin-integral.md) measure satisfying $\int d\bar\eta\,d\eta\,\bar\eta\eta=-1$ for one pair,

$$
\mathbf1=\int D(\bar\eta,\eta)e^{-\bar\eta\eta}|\eta\rangle\langle\bar\eta|,\qquad \operatorname{Tr}O=\int D(\bar\eta,\eta)e^{-\bar\eta\eta}\langle-\bar\eta|O|\eta\rangle
$$

for an even operator $O$; this is the [fermionic coherent-state trace](../../../../../fermionic-coherent-state-trace.md). In one mode the [trace](../../../../../matrix-trace.md) integrand is $e^{-\bar\eta\eta}(O_{00}-\bar\eta\eta O_{11})$, whose integral is $O_{00}+O_{11}$. Without the sign reversal it would be the [supertrace](../../../../../supertrace.md), not the thermal [trace](../../../../../matrix-trace.md). These formal Grassmann-valued [coherent states](../../../../../coherent-state.md) do not represent ordinary complex-valued [fermion](../../../../../fermion.md) amplitudes.

To construct the many-body thermal [path integral](../../../../../path-integral.md), write $\mathcal Z=\operatorname{Tr}e^{-\beta K}$ with $K=H-\mu\hat N$ and divide the imaginary-time interval $\mathcal T=\beta\hbar$ into slices of width $\delta\tau$. Insert the appropriate [coherent-state resolution of identity](../../../../../coherent-state-resolution-of-identity.md) between factors. For a normal-ordered [Hamiltonian](../../../../../hamiltonian.md), the adjacent-slice kernel is

$$
\langle\bar\psi_{j+1}|e^{-\delta\tau K/\hbar}|\psi_j\rangle=\exp\left[\bar\psi_{j+1}\psi_j-\frac{\delta\tau}{\hbar}K_N(\bar\psi_{j+1},\psi_j)+O(\delta\tau^2)\right].
$$

[coherent-state time slicing](../../../../../coherent-state-time-slicing.md) makes the overlap and [Gaussian measure](../../../../../gaussian-measure.md) combine into the first-order time derivative. The [grand-canonical coherent-state action](../../../../../grand-canonical-coherent-state-action.md) in the regulated [continuum limit](../../../../../continuum-limit.md) is

$$
\boxed{\mathcal Z=\int\mathcal D(\bar\psi,\psi)\,e^{-S_E/\hbar},\qquad S_E=\int_0^{\beta\hbar}d\tau\left[\hbar\sum_i\bar\psi_i\partial_\tau\psi_i+H_N(\bar\psi,\psi)-\mu\sum_i\bar\psi_i\psi_i\right].}
$$

For [bosons](../../../../../boson.md) the integration variables are complex, with the conjugate labels on the original integration contour; for [fermions](../../../../../fermion.md) the barred and unbarred [Grassmann variables](../../../../../grassmann-variable.md) are independent. The continuum notation retains the time-sliced ordering prescription. For example, $n(n-1)=a^{\dagger2}a^2$ has normal symbol $\bar z^2z^2$, whereas $n^2$ has that symbol plus $\bar zz$. Dropping that distinction changes a theory. The [coherent-state thermal boundary conditions](../../../../../coherent-state-thermal-boundary-conditions.md) follow because the bosonic [trace](../../../../../matrix-trace.md) closes paths periodically and the fermionic sign in the [trace](../../../../../matrix-trace.md) closes them antiperiodically:

$$
\psi(\beta\hbar)=\psi(0)\quad\text{(bosons)},\qquad \psi(\beta\hbar)=-\psi(0)\quad\text{(fermions)}.
$$

The barred fields obey the same respective boundary conditions. Hence [Matsubara frequencies](../../../../../matsubara-frequency.md) are $2\pi n/(\beta\hbar)$ and $(2n+1)\pi/(\beta\hbar)$. The derivative term encodes the canonical structure; omitting it would remove the quantum dynamics.[§§3.1–3.2, printed pp.51–61: coherent-state completeness, time slicing and fermionic trace boundary conditions](../../../../../physics-215c-quantum-field-theory-part-3-by-john-mcgreevy.md)

As a check, a free diagonal mode with $K=\xi a^\dagger a$ gives $Z_B=(1-e^{-\beta\xi})^{-1}$ for $\xi>0$, whereas $K=\xi c^\dagger c$ gives $Z_F=1+e^{-\beta\xi}$. Gaussian integration produces an inverse [determinant](../../../../../determinant.md) for [bosons](../../../../../boson.md) and a [determinant](../../../../../determinant.md) for independent complex [fermions](../../../../../fermion.md), with their respective temporal boundary conditions. Differentiating $\log Z$ recovers Bose-Einstein and Fermi-Dirac occupations. Interactions become higher powers in the normal-ordered symbols, and sources generate time-ordered correlations. **The coherent-state construction preserves statistics, ordering and boundary conditions together; a formal continuum expression without its measure and temporal prescription is incomplete.**

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
