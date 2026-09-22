<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

If $H|_L$ is constant, then $dH(v)=0$ for every $v\in TL$. By the definition of the [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md),

$$
\omega(X_H,v)=-dH(v)=0.
$$

Since $L$ is [Lagrangian](../../../../../lagrangian-submanifold.md), $(TL)^\omega=TL$, so $X_H$ is tangent to $L$. Its [Hamiltonian flow](../../../../../hamiltonian-isotopy.md) preserves $L$. This is the [Hamiltonian flow preserves a constant-level Lagrangian](../../../../../hamiltonian-flow-preserves-a-constant-level-lagrangian.md) principle.

The cotangent lift is functorial:

$$
(f\circ g)_\#=f_\#\circ g_\#.
$$

Since $\phi_{t+s}=\phi_t\circ\phi_s$, it follows that

$$
\psi_{t+s}=(\phi_{t+s})_\#=(\phi_t)_\#\circ(\phi_s)_\#=\psi_t\circ\psi_s.
$$

Thus $(\psi_t)$ is a flow with infinitesimal vector field $V_\#$ as stated in the question.

Finally, a cotangent lift sends the [conormal bundle](../../../../../conormal-bundle.md) $N^*Y$ to $N^*f(Y)$. Explicitly, if $\xi$ annihilates $T_xY$, then $(df_x^{-1})^*\xi$ annihilates $T_{f(x)}f(Y)$. Since $\phi_t(Y)=Y$, we have

$$
\psi_t(N^*Y)=N^*\phi_t(Y)=N^*Y,
$$

so the conormal bundle is invariant.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 140](../../paper-140-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
