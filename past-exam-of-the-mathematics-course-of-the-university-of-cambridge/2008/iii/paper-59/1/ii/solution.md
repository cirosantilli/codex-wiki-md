<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [fractal geometry](../../../../../../fractal-geometry.md), let $C_n$ be the $n$th middle-third construction of the [Cantor set](../../../../../../cantor-set.md). It contains $2^n$ intervals of length $3^{-n}$, with total length $(2/3)^n$. Each finite $C_n$ contains intervals, so its [Hausdorff dimension](../../../../../../hausdorff-dimension.md) is one. The limiting set $C=\bigcap_nC_n$ has zero length and

$$
\boxed{\dim_H C=\frac{\log2}{\log3}.}
$$

Indeed, $2^n$ intervals of scale $3^{-n}$ cover it, giving the upper dimension bound from $2^n3^{-ns}\to0$ whenever $s>\log2/\log3$. For the lower bound, assign mass $2^{-n}$ to each level-$n$ interval. Any sufficiently small interval of length $r$ meets only a bounded number of construction intervals at the comparable scale, giving a bound $\mu(I)\le Kr^{\log2/\log3}$. Covering $C$ by such intervals then forces their dimension-weighted sizes to sum to at least $1/K$, yielding the matching lower bound. The noninteger dimension is deducible from a simple iterative rule even though it is absent from every finite-stage set at arbitrarily fine resolution. A finite construction nevertheless exhibits the same scaling over intermediate resolutions. Thus the order of idealization and probing ever smaller scales matters: an actual finite-resolution pattern can have useful fractal behaviour without possessing the exact limiting dimension at all scales.

For a [phase transition](../../../../../../phase-transition.md), finite-spin [partition functions](../../../../../../canonical-partition-function.md) are finite sums of positive exponentials at real finite temperature and field. Their [free energies](../../../../../../thermodynamic-free-energy.md) are therefore analytic there. Genuine thermodynamic nonanalyticity can appear only after a suitable infinite-system limit. The [Curie–Weiss model](../../../../../../curie-weiss-model.md) gives an explicit demonstration. With $s_i=\pm1$, take

$$
H_N=-\frac{J}{2N}\left(\sum_i s_i\right)^2-h\sum_i s_i,\qquad J>0,\qquad\beta=(k_BT)^{-1}.
$$

Grouping configurations by $m=N^{-1}\sum_i s_i$ and using their binomial multiplicities gives the limiting [free energy](../../../../../../thermodynamic-free-energy.md) as the minimum of

$$
f(m)=-\frac J2m^2-hm-\beta^{-1}s(m),\qquad s(m)=-\frac{1+m}{2}\log\frac{1+m}{2}-\frac{1-m}{2}\log\frac{1-m}{2}.
$$

The number of possible magnetizations grows only linearly with $N$, so their largest exponential contribution determines the limiting [free energy](../../../../../../thermodynamic-free-energy.md). Differentiating the variational expression gives

$$
m=\tanh\{\beta(Jm+h)\}.
$$

At $h=0$ and $\beta J>1$, its two stable minima have magnetizations $\pm m_*\ne0$. Every finite zero-field system instead has exactly zero mean magnetization by spin-inversion [symmetry](../../../../../../symmetry-physics.md). Consequently

$$
\boxed{\lim_{h\downarrow0}\lim_{N\to\infty}\langle m\rangle_{N,h}=m_*,\qquad\lim_{N\to\infty}\lim_{h\downarrow0}\langle m\rangle_{N,h}=0.}
$$

This noncommutation of limits explains how [spontaneous symmetry breaking](../../../../../../spontaneous-symmetry-breaking.md) emerges. Below the critical temperature, the limiting [free energy](../../../../../../thermodynamic-free-energy.md) has a cusp in $h$ at zero, while finite systems have a sharp but smooth crossover. Away from the critical point, the relative weights of the two phases behave approximately as $e^{2\beta Nhm_*}$; the rounded magnetization is correspondingly about $m_*\tanh(\beta Nhm_*)$. Exact singularity belongs to the idealized limit, whereas the narrow crossover and long-lived phases can be physically useful at finite size. The [theoretical reduction](../../../../../../theoretical-reduction.md) is the derivation and its approximation control, not a claim that a finite analytic [partition function](../../../../../../canonical-partition-function.md) is already nonanalytic.

For [superselection](../../../../../../superselection-rule.md), consider an infinite spin lattice with [quasi-local observable algebra](../../../../../../quasi-local-observable-algebra.md) $\mathcal A$. These are zero-temperature equilibrium phases of a ferromagnetic Ising spin Hamiltonian with nearest-neighbour interactions $-J\sigma_z^{(i)}\sigma_z^{(j)}$. At finite $N$, the all-up and all-down vectors belong to one Hilbert space, and the coherent state

$$
|\Psi_N\rangle=\frac{|\uparrow\cdots\uparrow\rangle+e^{i\theta}|\downarrow\cdots\downarrow\rangle}{\sqrt2}
$$

is distinguishable from the corresponding mixture by a suitably chosen global [observable](../../../../../../observable.md). But if $A_R$ acts on only $R<N$ spins, its off-diagonal matrix element between these vectors vanishes: the untouched spins contribute $\langle\uparrow|\downarrow\rangle=0$. Hence its expectations already equal those of the equal-weight mixture, independent of $\theta$. Increasingly global [observables](../../../../../../observable.md) can recover the phase at finite $N$, but the infinite product of spin flips is not a norm limit of finite-support [observables](../../../../../../observable.md) and is absent from $\mathcal A$.

In the infinite-volume limit the up and down phases have disjoint state representations. The averaged magnetization $M_N=N^{-1}\sum_i\sigma_z^{(i)}$ commutes asymptotically with any fixed local [observable](../../../../../../observable.md): $\|[M_N,A_R]\|\le2R\|A_R\|/N$. In the phase representations its limiting values are $+1$ and $-1$, distinguishing sectors. Finite spin-flip vectors form a dense set on which these averages tend to their respective scalar values, so boundedness extends the strong limits to the phase Hilbert spaces. An intertwiner between the representations would obey $(-I)T=T(+I)$ and must therefore vanish, explaining their disjointness. In the combined representation the [observable](../../../../../../observable.md) algebra is block-diagonal between them, so no quasilocal measurement detects their relative phase. This yields an emergent [superselection rule](../../../../../../superselection-rule.md) relative to the chosen [observable](../../../../../../observable.md) algebra. It is not a derivation of physical wave-function collapse. **Fractal dimension, a thermodynamic singularity and sector separation each exhibit new limiting structure while retaining an explicit microscopic construction.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
