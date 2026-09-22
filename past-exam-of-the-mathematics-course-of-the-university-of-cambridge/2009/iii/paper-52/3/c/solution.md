<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the driving and feedback strengths to be real, so the feedback [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) is Hermitian. The lowering operator satisfies $\sigma^2=(\sigma^\dagger)^2=0$. Using the supplied convention for $\sigma_y$,

$$
\sigma^\dagger\sigma_y=i\sigma^\dagger\sigma,\qquad
\sigma_y\sigma=-i\sigma^\dagger\sigma.
$$

The additional [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) term is consequently

$$
\tfrac12(M^\dagger F+FM)
=\tfrac\lambda2(\sigma^\dagger\sigma_y+\sigma_y\sigma)=0.
$$

With no drift [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md), the total [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) is just $\alpha\sigma_y$. The feedback-modified [Lindblad operator](../../../../../../lindblad-operator.md) is

$$
K=\sigma-i\lambda\sigma_y=(1+\lambda)\sigma-\lambda\sigma^\dagger
=\begin{pmatrix}0&1+\lambda\\-\lambda&0\end{pmatrix}.
$$

Substitution into the measurement-feedback equation gives

$$
\boxed{\dot\rho=-i[\alpha\sigma_y,\rho]+\mathcal D[K]\rho.}
$$

Thus the feedback affects the [Lindblad dissipator](../../../../../../lindblad-dissipator.md) even though its extra coherent [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) contribution cancels. This is a concrete mechanism of [Markovian reservoir engineering](../../../../../../markovian-reservoir-engineering.md), rather than merely a classical control force added to an unchanged dissipative equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
