# Conditional input ensemble after a local measurement

↑ **Parent:** [Measurement channel](measurement-channel.md)

For a bipartite input [density operator](density-matrix.md) $\rho^x_{AC}$ and a [POVM](positive-operator-valued-measure.md) $\{E_y\}$ on $A$, let $q(y|x)=\operatorname{Tr}[(E_y\otimes I)\rho^x]$. For $q(y|x)>0$, the conditioned input on $C$ is

$$
\rho_C^{x,y}=\frac{\operatorname{Tr}_A[(\sqrt{E_y}\otimes I)\rho^x(\sqrt{E_y}\otimes I)]}{q(y|x)}.
$$

Its positivity follows from the positive sandwich before the [partial trace](partial-trace.md). A [quantum channel](quantum-channel.md) on $C$ acts on these conditional [density operators](density-matrix.md) even if the original input is an [entangled state](entangled-state.md).

## ↑ Ancestors (7)

1. [Measurement channel](measurement-channel.md)
2. [Measure-and-prepare channel](measure-and-prepare-channel.md)
3. [Quantum information theory](quantum-information-theory-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Holevo-capacity additivity for entanglement-breaking channels](holevo-capacity-additivity-for-entanglement-breaking-channels.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/1/ii/solution.md)
