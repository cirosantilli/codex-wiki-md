# Eigenbasis proof of quantum relative entropy nonnegativity

↑ **Parent:** [Nonnegativity of quantum relative entropy](nonnegativity-of-quantum-relative-entropy.md)

Diagonalize two [density operators](density-matrix.md) with eigenvalues $r_i,s_j$, and put $q_{ij}=|\langle i|j\rangle|^2$. This overlap matrix has row and column sums one. The scalar inequality $u\ln(u/v)\ge u-v$ yields $D(\rho\|\sigma)\ge\sum_{ij}q_{ij}(r_i-s_j)=0$ in natural units; division by $\ln2$ gives bits. Equality forces $r_i=s_j$ whenever $q_{ij}>0$, so $\sigma|i\rangle=r_i|i\rangle$ and $\rho=\sigma$. Zero eigenvalues use limits, and failure of support inclusion gives infinite [quantum relative entropy](quantum-relative-entropy.md).

## ↑ Ancestors (8)

1. [Nonnegativity of quantum relative entropy](nonnegativity-of-quantum-relative-entropy.md)
2. [Quantum relative entropy](quantum-relative-entropy.md)
3. [Von Neumann entropy](von-neumann-entropy-split.md)
4. [Density matrix](density-matrix.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
