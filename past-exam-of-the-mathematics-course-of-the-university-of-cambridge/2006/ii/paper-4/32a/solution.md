<h1 id="32a/solution">Solution</h1>

↑ **Parent:** [32A](../32a.md)

Let $U(t,t_0)$ be the unitary Schrödinger propagator. The Heisenberg state is fixed at its initial value, while $A_H=U^\dagger A_SU$. Since $\psi_S(t)=U\psi_H$, matrix elements and probabilities agree exactly in the two pictures. Differentiating, for an operator with no explicit Schrödinger-time dependence, gives

$$
\boxed{\dot A_H=\frac i\hbar[H_H,A_H]}.
$$

For constant [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), $U=e^{-iH(t-t_0)/\hbar}$ and $H_H=H$.

A spatial rotation is represented by $U_R(\theta)=\exp[-i\theta n\cdot J/\hbar]$, where $J$ is the total [angular momentum operator](../../../../../angular-momentum-operator.md). For a particle $J=L+S$. The commutators $[J_i,x_j]=i\hbar\epsilon_{ijk}x_k$ and $[J_i,S_j]=i\hbar\epsilon_{ijk}S_k$ give

$$
U_R^\dagger xU_R=x+\theta n\times x+O(\theta^2),\qquad
U_R^\dagger SU_R=S+\theta n\times S+O(\theta^2).
$$

These are the correct infinitesimal vector rotations, verifying the generator and sign.

For the specified [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), $p^2$ and $x^2$ commute with every $J_i$. Moreover

$$
[J_i,x\cdot S]=i\hbar\sum_{j,k}\epsilon_{ijk}(x_kS_j+x_jS_k)=0
$$

by antisymmetry. Thus $[J_i,H]=0$ and **every total-angular-momentum component is constant in the [Heisenberg picture](../../../../../heisenberg-picture.md)**. The separate torques are

$$
\boxed{\dot L=-U(x^2)x\times S,\qquad \dot S=+U(x^2)x\times S}.
$$

They cancel but need not vanish individually, so orbital and [spin angular momentum](../../../../../spin.md) are generally not separately conserved.

## ↑ Ancestors (10)

1. [32A](../32a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
