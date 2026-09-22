<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add a nonconducting inactivated state to the [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md):

$$
C\mathrel{\mathop{\rightleftarrows}^{k_o(V)}_{k_c(V)}}O
\mathrel{\mathop{\rightleftarrows}^{k_i(V)}_{k_r(V)}}I,
\qquad p_C+p_O+p_I=1.
$$

For example, $\dot p_O=k_op_C-(k_c+k_i)p_O+k_rp_I$ and $\dot p_I=k_ip_O-k_rp_I$. [Depolarization](../../../../depolarization.md) first increases $p_O$, then transfers population into $I$ by [ball-and-chain inactivation](../../../../ball-and-chain-inactivation.md). A small recovery rate during the pulse permits a sustained decline of $I_K=N\gamma p_O(V-E_K)$. [Repolarization](../../../../repolarization.md) favors recovery, eventually restoring the closed but available population. Several sequential closed states can represent the cooperative movements of four [voltage-sensing domains](../../../../voltage-sensing-domain.md); three states are the minimal explanation of rise followed by decay, rather than a quantitative fit to the missing trace.

Loss of outward [potassium](../../../../potassium.md) [electric current](../../../../electric-current.md) weakens [repolarization](../../../../repolarization.md) and can broaden an [action potential](../../../../action-potential.md). Reduced residual [potassium](../../../../potassium.md) [electrical conductance](../../../../electrical-conductance.md) can reduce the subsequent [hyperpolarization](../../../../hyperpolarization.md) and permit faster repeated firing. Conversely, prolonged [depolarization](../../../../depolarization.md) can maintain [sodium](../../../../sodium.md) [ion-channel inactivation](../../../../ion-channel-inactivation.md), delay recovery and lower the maximum firing frequency or cause depolarization block. The sign of the frequency change depends on the other [ion channels](../../../../ion-channel.md) and recovery kinetics; rapid [potassium](../../../../potassium.md) [ion-channel inactivation](../../../../ion-channel-inactivation.md) alone does not fix it.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
