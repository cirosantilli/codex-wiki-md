# Transfer matrix of a delta potential

↑ **Parent:** [Delta potential](delta-potential.md)

For $V(x)=g\delta(x-x_0)$, put $q=\sqrt{2mE}/\hbar>0$ and $\gamma=mg/(\hbar^2q)$. Relate the coefficients of $Ae^{iqx}+Be^{-iqx}$ immediately to the right and left by $v_R=D(x_0)v_L$. Continuity of the [wavefunction](wave-function-split.md) and integration of the [Schrödinger equation](schrodinger-equation.md) across the [delta potential](delta-potential.md) give $\psi'(x_0^+)-\psi'(x_0^-)=2mg\psi(x_0)/\hbar^2$. Solving these two matching equations gives

$$
D(x_0)=\begin{pmatrix}1-i\gamma&-i\gamma e^{-2iqx_0}\\i\gamma e^{2iqx_0}&1+i\gamma\end{pmatrix},\qquad\det D(x_0)=1.
$$

For scatterers at $x_1<\cdots<x_N$, the full [transfer matrix](transfer-matrix.md) is $M=D(x_N)\cdots D(x_1)$: the leftmost scatterer acts first on the coefficient column. With these globally phased [plane waves](plane-wave.md), the propagation phases are already in each $D(x_j)$. For incidence only from the left, $t=1/M_{22}$ and $r=-M_{21}/M_{22}$ follow from $(t,0)^T=M(1,r)^T$ and $\det M=1$.

## ↑ Ancestors (5)

1. [Delta potential](delta-potential.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-further-quantum-theory-course-of-the-university-of-oxford/2023/2/c/solution.md)
