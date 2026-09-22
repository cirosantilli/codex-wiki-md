<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

The [chemical potential](../../../../../chemical-potential.md) is $\mu=(\partial E/\partial N)_{S,V}$, equivalently $(\partial F/\partial N)_{T,V}$: it is the free-energy cost of adding a particle at fixed temperature and volume. With units $k_B=1$, a large reservoir has entropy $S_R(E_{\rm tot}-E,N_{\rm tot}-N)=S_R^0-E/T+\mu N/T$ to first order. Since the number of compatible reservoir states is proportional to its exponential, the [grand canonical ensemble](../../../../../grand-canonical-ensemble.md) assigns

$$
\boxed{\Pr(\text{state }j,N)=\Xi^{-1}e^{-(E_{j,N}-\mu N)/T},\quad\Xi=\sum_{N,j}e^{-(E_{j,N}-\mu N)/T}.}
$$

For independent [fermions](../../../../../fermion.md), a one-particle state of energy $\varepsilon$ has occupation zero or one. Its partition factor is $1+e^{-(\varepsilon-\mu)/T}$, so the mean occupation is the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) $[e^{(\varepsilon-\mu)/T}+1]^{-1}$. Multiplication by the given [density of states](../../../../../density-of-states.md) yields $dN=C\varepsilon^{1/2}d\varepsilon/[e^{(\varepsilon-\mu)/T}+1]$.

At zero temperature the occupation is a step function, filled below $\mu$ and empty above it, so $\mu=\varepsilon_F$ and $N=(2C/3)\varepsilon_F^{3/2}$. At fixed particle number, the low-temperature shift of $\mu$ is $O(T^2/\varepsilon_F)$ and does not affect the leading estimate. In the narrow interval of width $T$ above $\varepsilon_F$, replace the density of states by $C\sqrt{\varepsilon_F}$ and put $u=(\varepsilon-\varepsilon_F)/T$. Then

$$
\boxed{N_{>\varepsilon_F}\sim C\sqrt{\varepsilon_F}\,T\int_0^\infty\frac{du}{e^u+1}=C\sqrt{\varepsilon_F}\,T\log2.}
$$

Equivalently, the fraction above the [Fermi energy](../../../../../fermi-energy.md) is asymptotic to $(3\log2/2)T/\varepsilon_F$.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
