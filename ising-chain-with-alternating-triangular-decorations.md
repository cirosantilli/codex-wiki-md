# Ising chain with alternating triangular decorations

↑ **Parent:** [Antiferromagnetic Ising model](antiferromagnetic-ising-model.md)

Take $2M$ base [Ising spins](ising-spin-variable.md) on a ring and add one apex [Ising spin](ising-spin-variable.md) over every other base bond. Give all base and apex bonds the antiferromagnetic [energy](energy-split.md) $Jss'$ with $J>0$. There are $3M$ sites, and adjacent triangles are connected by a single undecorated bridge rather than sharing a corner. With $K=J/(k_BT)$, summing the apex spins yields alternating [spin-chain transfer matrices](transfer-matrix-for-a-classical-spin-chain.md)

$$
A_{st}=2e^{-Kst}\cosh[K(s+t)],\qquad B_{st}=e^{-Kst},\qquad Z=\operatorname{Tr}(AB)^M.
$$

Their common symmetric [eigenvector](eigenvector.md) gives the leading cell [eigenvalue](eigenvalue.md) $3+e^{-4K}+e^{-2K}+3e^{2K}$. A minimum-energy triangle has one frustrated bond and [energy](energy-split.md) $-J$; its connecting bridge can have [energy](energy-split.md) $-J$. Requiring the bridge to be antiparallel leaves the counting [transfer matrix](transfer-matrix.md) $\left(\begin{smallmatrix}2&1\\1&2\end{smallmatrix}\right)$ on successive first base spins. Its [eigenvalues](eigenvalue.md) $3,1$ give [ground-state degeneracy](ground-state-degeneracy.md) $g_M=3^M+1$ and [ground-state energy](ground-state-energy.md) $-2JM$. The [residual entropy](residual-entropy.md) per site is $k_B\ln3/3$.

## ↑ Ancestors (7)

1. [Antiferromagnetic Ising model](antiferromagnetic-ising-model.md)
2. [Ising model](ising-model.md)
3. [Spin model](spin-model-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford/2018/2/c/solution.md)
- [Solution](past-exam-of-the-advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford/2018/2/d/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-major-option-course-of-the-university-of-oxford/2018/4/c/solution.md)
