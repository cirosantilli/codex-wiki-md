<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The usual sufficient input promises for the [HHL algorithm](../../../../../../../hhl-algorithm.md) are efficient [quantum state preparation](../../../../../../../quantum-state-preparation.md) of the nonzero vector $b$, efficient access to a [sparse matrix](../../../../../../../sparse-matrix.md) $A$ with at most $\operatorname{poly}(n)$ nonzero entries per row, and a [condition number](../../../../../../../condition-number.md) $\kappa=\lambda_{\max}/\lambda_{\min}=\operatorname{poly}(n)$ after an efficiently known normalization. Both the positions and values of the nonzero [matrix elements](../../../../../../../matrix-element.md) must be computable coherently in [polynomial time](../../../../../../../polynomial-time.md). More generally, efficient [Hamiltonian simulation](../../../../../../../hamiltonian-simulation.md) can replace the sparsity promise. We assume $A$ is invertible; if zero [eigenvalues](../../../../../../../eigenvalue.md) occur, one must instead restrict $b$ to their [orthogonal complement](../../../../../../../orthogonal-complement.md) and specify the desired inverse on that support.

With $a=\lambda_{\max}$ and a known bound $\kappa$, choose $c=a/\kappa\leq\lambda_{\min}$. The [HHL controlled reciprocal rotation](../../../../../../../hhl-controlled-reciprocal-rotation.md) then succeeds with probability

$$
p_{\rm succ}=c^2\|A^{-1}|b\rangle\|^2\geq\frac{c^2}{a^2}=\boxed{\kappa^{-2}}.
$$

This is the required inverse-polynomial lower bound. In the usual approximate algorithm, inverse-polynomial requested error also gives polynomial runtime under these input promises. The original [HHL paper](https://arxiv.org/abs/0811.3171) states the dependence on sparsity, conditioning, and accuracy.

There is a qualification for a literally exact version. Representability of the [eigenvalues](../../../../../../../eigenvalue.md) in $n$ bits does not itself make exact [quantum phase estimation](../../../../../../../quantum-phase-estimation.md) efficient: using $e^{2\pi iA}$ requires controlled powers corresponding to evolution times as large as $2\pi2^{n-1}$. Under the paper's idealization we may describe their exact action, but polynomial runtime for that exact circuit additionally requires efficient implementations of those controlled powers, or equivalent efficient exact spectral access. Assuming an operation executes exactly does not bound its cost. This distinction is recorded in [cost of exact phase estimation on a dyadic spectrum](../../../../../../../cost-of-exact-phase-estimation-on-a-dyadic-spectrum.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
