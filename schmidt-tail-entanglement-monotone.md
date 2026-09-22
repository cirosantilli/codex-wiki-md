# Schmidt-tail entanglement monotone

↑ **Parent:** [Entanglement monotone](entanglement-monotone.md)

For a bipartite [pure state](pure-state.md), the squared [Schmidt coefficients](schmidt-coefficient.md) are the nonzero [eigenvalues](eigenvalue.md) of either [reduced density matrix](reduced-density-matrix.md). Their sum except the largest defines $E_2=1-\lambda_{\max}(\rho_A)$. The largest eigenvalue is a convex function, since $\lambda_{\max}(\rho)=\max_{\|v\|=1}\langle v|\rho|v\rangle$; consequently $E_2$ is concave. If Alice measures locally and records outcome $r$, Bob's conditional reductions satisfy $\sum_r p_r\rho_{B,r}=\rho_B$. Concavity gives $\sum_r p_rE_2(\chi_r)\leq E_2(\chi)$. For Bob's measurements use Alice's unchanged average reduction instead. Iteration proves average monotonicity under [LOCC](local-operations-and-classical-communication.md). For [Schmidt rank](schmidt-rank.md) at most two, $E_2$ is the smaller squared Schmidt coefficient. A conversion succeeding with probability $p$ therefore obeys $pE_2(\phi)\leq E_2(\psi)$, since failure branches contribute nonnegative amounts.

## ↑ Ancestors (8)

1. [Entanglement monotone](entanglement-monotone.md)
2. [Entangled state](entangled-state.md)
3. [Reduced density matrix](reduced-density-matrix.md)
4. [Bell state](bell-state-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Optimal stochastic conversion of a two-qubit pure state](optimal-stochastic-conversion-of-a-two-qubit-pure-state.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/b/solution.md)
