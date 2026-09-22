<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [periodic boundary condition](../../../../periodic-boundary-conditions.md) requires $e^{ikM}=1$, so there are exactly $M$ independent [wavevectors](../../../../wavevector.md) in a [Brillouin zone](../../../../brillouin-zone.md):

$$
\boxed{k=\frac{2\pi l}{M},\qquad l=0,\ldots,M-1\quad(\bmod\ 2\pi).}
$$

The inverse [discrete Fourier transform](../../../../discrete-fourier-transform-split.md), with the sign convention of the paper, is

$$
c^\dagger_{\sigma,j}=\frac1{\sqrt M}\sum_k e^{-ikj}\widetilde c^\dagger_{\sigma,k},\qquad
c_{\sigma,j}=\frac1{\sqrt M}\sum_k e^{ikj}\widetilde c_{\sigma,k}.
$$

[Fourier orthogonality](../../../../fourier-orthogonality.md) gives the [tight binding](../../../../tight-binding.md) [dispersion relation](../../../../dispersion-relation-split.md) $\epsilon_k=-2t\cos k$. For the interaction, first use the [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) at distinct sites to write $n_{\sigma,j}n_{\sigma,j+1}=c^\dagger_{\sigma,j}c^\dagger_{\sigma,j+1}c_{\sigma,j+1}c_{\sigma,j}$. Summing its [discrete Fourier transform](../../../../discrete-fourier-transform-split.md) over $j$ enforces [crystal momentum conservation](../../../../crystal-momentum-conservation.md), giving

$$
\boxed{H=\sum_{\sigma,k}(-2t\cos k)\widetilde c^\dagger_{\sigma,k}\widetilde c_{\sigma,k}
+\frac VM\sum_{\sigma,k,p,q}e^{iq}\widetilde c^\dagger_{\sigma,k+q}\widetilde c^\dagger_{\sigma,p-q}\widetilde c_{\sigma,p}\widetilde c_{\sigma,k}.}
$$

Every [wavevector](../../../../wavevector.md) is reduced modulo $2\pi$. The phase $e^{iq}$ comes from the displacement of the second site by one lattice spacing. Equivalently replace $e^{iq}$ by $\cos q$: exchanging the two incoming and the two outgoing [fermions](../../../../fermion.md) changes $q$ to $-q$ with two cancelling [fermionic signs](../../../../fermionic-sign.md). Thus the usual interaction vertex is $2V\cos q$ accompanied by the factor $1/(2M)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
