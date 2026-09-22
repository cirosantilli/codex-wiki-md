<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the scalar two-particle model, the [fermionic exchange symmetry](../../../../fermi-dirac-statistics.md) and [bosonic exchange symmetry](../../../../bosonic-exchange-symmetry.md) conditions are

$$
\boxed{\Psi(x_2,x_1)=-\Psi(x_1,x_2)\text{ for fermions},\qquad
\Psi(x_2,x_1)=\Psi(x_1,x_2)\text{ for bosons}.}
$$

For particles with spin, exchange acts on all their labels; the stated coordinate-only model fixes the spatial symmetry sector. Define $S\Psi(x_1,x_2)=\Psi(x_2,x_1)$. Equal masses make the kinetic operator invariant under exchange, and the assumed potential is invariant too, so $HS=SH$. Therefore $H\Psi=E\Psi$ implies $H(S\Psi)=E(S\Psi)$. The components

$$
\Psi_{\mathrm B}=\tfrac12(\Psi+S\Psi),\qquad
\Psi_{\mathrm F}=\tfrac12(\Psi-S\Psi)
$$

are respectively symmetric and antisymmetric eigenfunctions whenever nonzero. Their sum is the original nonzero [quantum state](../../../../quantum-state.md), so at least one is nonzero. An eigenspace may contain both sectors if the energy is degenerate.

The [normal modes of two harmonically coupled identical particles](../../../../normal-modes-of-two-harmonically-coupled-identical-particles.md) provide the separation. The [coordinate transformation](../../../../smooth-transition-map.md) to $y_+,y_-$ is [orthogonal](../../../../orthogonal-vectors.md), with absolute Jacobian one. Exchanging the particles leaves $y_+$ fixed and changes $y_-$ to $-y_-$. Hence **bosonic [quantum states](../../../../quantum-state.md) are even and fermionic [quantum states](../../../../quantum-state.md) odd in the relative coordinate**. The [chain rule](../../../../chain-rule.md) gives

$$
\partial_{x_1}=\frac{\partial_{y_+}+\partial_{y_-}}{\sqrt2},\qquad
\partial_{x_2}=\frac{\partial_{y_+}-\partial_{y_-}}{\sqrt2},\qquad
\partial_{x_1}^2+\partial_{x_2}^2=\partial_{y_+}^2+\partial_{y_-}^2.
$$

Also $x_1^2+x_2^2=y_+^2+y_-^2$ and $(x_1-x_2)^2=2y_-^2$. Combining the two trapping potentials with the interaction therefore gives the separated [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md)

$$
H=\left[-\frac{\hbar^2}{2m}\partial_{y_+}^2+\frac12m\omega^2y_+^2\right]
+\left[-\frac{\hbar^2}{2m}\partial_{y_-}^2+\frac12m\omega^2\cos^2\alpha\,y_-^2\right].
$$

These are independent oscillators of frequencies $\omega$ and $\omega\cos\alpha$. Both frequencies are positive in the stated range. Their product [eigenstates](../../../../eigenstate.md) have energies

$$
\boxed{E_{n_+,n_-}=\hbar\omega\left[n_++\tfrac12+(n_-+\tfrac12)\cos\alpha\right],\qquad n_+,n_-=0,1,2,\ldots.}
$$

The [parity](../../../../parity.md) of an oscillator level is $(-1)^n$. Consequently [bosons](../../../../boson.md) allow even $n_-$ and [fermions](../../../../fermion.md) odd $n_-$, while $n_+$ is unrestricted.

The bosonic [ground state](../../../../ground-state.md) uses $n_+=n_-=0$, and the fermionic [ground state](../../../../ground-state.md) uses $n_+=0,n_-=1$. The oscillator length in the relative mode is

$$
\boxed{\tau^2=\frac{\hbar}{m\omega\cos\alpha}=\frac{\hbar\sec\alpha}{m\omega}.}
$$

Using the normalized [Gaussian](../../../../normal-distribution.md) for each mode gives

$$
\boxed{\Phi_{\mathrm B}(y_+,y_-)=\psi_\sigma(y_+)\psi_\tau(y_-),\qquad
\Phi_{\mathrm F}(y_+,y_-)=\psi_\sigma(y_+)\phi_\tau(y_-).}
$$

Indeed $\phi_\tau(y)=\sqrt2\,y\psi_\tau(y)/\tau$ by differentiating the [Gaussian](../../../../normal-distribution.md), so it is the normalized odd first [excited state](../../../../excited-state.md). The ground energies are $E_{\mathrm B}=\hbar\omega(1+\cos\alpha)/2$ and $E_{\mathrm F}=\hbar\omega(1+3\cos\alpha)/2$.

Choose normalized factors for a normalized product [quantum state](../../../../quantum-state.md); this can always be done by reciprocal rescaling of its factors. Since the coordinate Jacobian has absolute value one,

$$
\mathbb E[f(y_-)]=\iint f(y_-)\,|\psi(y_+)|^2|\phi(y_-)|^2\,dy_+dy_-
=\boxed{\int f(y)|\phi(y)|^2\,dy.}
$$

If the supplied factors are not individually normalized, the general expression has an additional factor $\|\psi\|^2$; choosing normalized factors is the convention in the displayed formula.

For the [ground states](../../../../ground-state.md), put $\rho(y)=|\psi_\tau(y)|^2=e^{-y^2/\tau^2}/(\sqrt\pi\tau)$. Then $|\phi_\tau(y)|^2=2y^2\rho(y)/\tau^2$ and $\rho'=-2y\rho/\tau^2$. Thus, for differentiable $f$ with suitable [Gaussian](../../../../normal-distribution.md) integrability and vanishing boundary terms,

$$
\mathbb E_{\mathrm F}[f]=\frac2{\tau^2}\int y^2f(y)\rho(y)\,dy
=-\int yf(y)\rho'(y)\,dy
=\boxed{\int\bigl(f(y)+yf'(y)\bigr)\rho(y)\,dy.}
$$

This is [integration by parts](../../../../integration-by-parts.md), and every polynomial satisfies the required endpoint conditions. The [relative-coordinate moments in even and odd oscillator ground states](../../../../relative-coordinate-moments-in-even-and-odd-oscillator-ground-states.md) follow by substituting $f(y)=y^n$:

$$
\boxed{\mathbb E_{\mathrm F}[y_-^n]=(n+1)\mathbb E_{\mathrm B}[y_-^n].}
$$

For odd $n$, both expectations vanish by [parity](../../../../parity.md), so this is an equality of zeros rather than an increase in signed mean separation. The even moments show the physical difference. In particular $\mathbb E_{\mathrm B}[y_-^2]=\tau^2/2$ and $\mathbb E_{\mathrm F}[y_-^2]=3\tau^2/2$, so the fermionic root-mean-square particle separation is $\sqrt3$ times the bosonic value. The fermionic [probability density](../../../../probability-density.md) vanishes at coincidence $y_-=0$, expressing [Pauli exclusion principle](../../../../pauli-exclusion-principle.md) in this spatial symmetry sector. This is an exchange constraint on the [wave function](../../../../wave-function-split.md), not an additional classical force. As $\alpha$ approaches $\pi/2$, the relative oscillator softens and its width diverges; the excluded endpoint would no longer have this normalizable oscillator [ground state](../../../../ground-state.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the quantum mechanics and electromagnetism course of the University of Oxford](../../../split.md)
5. [Quantum mechanics and electromagnetism course of the University of Oxford](../../../../quantum-mechanics-and-electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
