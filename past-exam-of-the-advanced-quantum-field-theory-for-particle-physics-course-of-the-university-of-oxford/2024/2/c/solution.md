<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the source's [charge-conjugation matrix](../../../../charge-conjugation-matrix.md) convention $C\gamma^\mu C^{-1}=-(\gamma^\mu)^T$. It implies

$$
C^{-1}(\gamma^\mu)^TC=-\gamma^\mu,\qquad
C^{-1}K(p)^TC=K(-p).
$$

A [trace](../../../../matrix-trace.md) equals the [trace](../../../../matrix-trace.md) of its [matrix transpose](../../../../transpose.md), which reverses the order of all factors. Inserting the displayed identities gives

$$
\begin{aligned}
T_A(\ell)&=\operatorname{tr}[\gamma^\mu K(\ell+k_1)\gamma^\nu K(\ell-k_3)\gamma^\rho K(\ell)]\\
&=-\operatorname{tr}[K(-\ell)\gamma^\rho K(-\ell+k_3)\gamma^\nu K(-\ell-k_1)\gamma^\mu]\\
&=-\operatorname{tr}[\gamma^\mu K(-\ell)\gamma^\rho K(-\ell+k_3)\gamma^\nu K(-\ell-k_1)].
\end{aligned}
$$

There is one minus sign from each of the three photon [interaction vertices](../../../../interaction-vertex.md), and none from the transformed [Dirac propagators](../../../../dirac-propagator.md). In the last line, change [loop momentum](../../../../loop-momentum.md) to $\ell'=-\ell-k_1$. Since $k_1+k_3=-k_2$, its three [Dirac propagators](../../../../dirac-propagator.md) become $K(\ell'+k_1)$, $K(\ell'-k_2)$, $K(\ell')$, exactly those of the reversed orientation. Hence

$$
\boxed{\mathcal M_A^{\mu\nu\rho}=-\mathcal M_B^{\mu\nu\rho},\qquad
\mathcal M_{\rm one\ loop}^{\mu\nu\rho}=0.}
$$

This is [Furry's theorem](../../../../furry-s-theorem.md). The [regularization in quantum field theory](../../../../regularization-in-quantum-field-theory.md) matters: the individual [Feynman integrals](../../../../feynman-integral.md) are superficially divergent, so an unregulated shift of a divergent integral is not a proof. A common [dimensional regularization](../../../../dimensional-regularization.md) preserves [charge conjugation](../../../../charge-conjugation.md) and the vector [Ward identity](../../../../ward-identity.md), making the change of variables legitimate. No [chirality matrix](../../../../chirality-matrix.md) occurs, so the axial triangle [anomaly](../../../../anomaly-physics.md) is not involved.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
