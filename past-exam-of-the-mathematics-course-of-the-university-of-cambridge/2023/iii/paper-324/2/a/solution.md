<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the [spectral decomposition](../../../../../../spectral-decomposition.md) of the Hermitian matrix be

$$
A=\sum_j\lambda_j|u_j\rangle\langle u_j|,
\qquad
|b\rangle=\sum_j\beta_j|u_j\rangle.
$$

The [HHL algorithm](../../../../../../hhl-algorithm.md) proceeds as follows.

[ Efficiently](https://ourbigbook.com/-/topic/efficiently) prepare the normalized amplitude encoding $|b\rangle$.  
[ Apply](https://ourbigbook.com/-/topic/apply) [quantum phase estimation](../../../../../../quantum-phase-estimation.md) to the simulated evolution $e^{iAt}$, producing an approximation of each eigenvalue:

$$
\sum_j\beta_j|u_j\rangle|\widetilde\lambda_j\rangle.
$$

[ Add](https://ourbigbook.com/-/topic/add) one ancilla and perform an eigenvalue-controlled rotation

$$
|\widetilde\lambda_j\rangle|0\rangle
\longmapsto
|\widetilde\lambda_j\rangle
\left(\sqrt{1-\frac{C^2}{\widetilde\lambda_j^2}}|0\rangle
+\frac{C}{\widetilde\lambda_j}|1\rangle\right),
$$

where $0<C\leq\min_j|\lambda_j|$.  
[ Uncompute](https://ourbigbook.com/-/topic/uncompute) the eigenvalue register. Conditional on measuring the ancilla as $1$, the system register is

$$
|x\rangle=
\frac{A^{-1}|b\rangle}{\|A^{-1}|b\rangle\|}
=\frac{\sum_j\beta_j\lambda_j^{-1}|u_j\rangle}
{\sqrt{\sum_j|\beta_j|^2|\lambda_j|^{-2}}}.
$$

The postselection probability can be increased with [amplitude amplification](../../../../../../amplitude-amplification.md).

The ingredients used here are efficient sparse [Hamiltonian simulation](../../../../../../hamiltonian-simulation.md) of $e^{iAt}$ and [quantum phase estimation](../../../../../../quantum-phase-estimation.md), which converts an eigenphase of that evolution into a binary approximation of $\lambda_j$. For sparsity $s$, condition number $\kappa$, and error $\epsilon$, the cost is polynomial in $s$, $\kappa$, $1/\epsilon$, and $\log N$ under the stated access assumptions.

Finally estimate $\langle x|M|x\rangle$ by repeated measurement of an efficient observable decomposition of $M$, or by a [Hadamard test](../../../../../../hadamard-test.md) when $M$ is unitary. A general efficiently block-encoded Hermitian $M$ can similarly be measured through its block encoding. Repetition and a [concentration inequality](../../../../../../concentration-inequality.md) give additive sampling error $O(1/\sqrt R)$ after $R$ independent preparations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
