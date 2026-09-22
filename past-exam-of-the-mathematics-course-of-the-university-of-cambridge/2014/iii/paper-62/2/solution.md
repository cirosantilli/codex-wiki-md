<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In an [ontological model of a quantum system](../../../../../ontological-model-of-a-quantum-system.md), a preparation of $|\psi\rangle$ gives a [probability distribution](../../../../../probability-distribution.md) $\mu_\psi$ over a physical state $\lambda$. A fixed [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) has response probabilities $\xi_j(\lambda)\geq0$ with $\sum_j\xi_j=1$, reproducing the [Born rule](../../../../../born-rule.md) after averaging over $\mu_\psi$. The [PBR theorem](../../../../../pusey-barrett-rudolph-theorem.md) says that, assuming [preparation independence](../../../../../preparation-independence.md) and the quantum predictions, distributions for distinct [pure states](../../../../../pure-state.md) cannot overlap with positive probability. Thus the [quantum state](../../../../../quantum-state.md) is determined by the physical state in the [psi-ontic model](../../../../../psi-ontic-model.md) sense.

[Preparation independence](../../../../../preparation-independence.md) says that separately prepared systems have independent physical states: a product preparation is represented by the product of their individual ontic distributions. This is an assumption about the underlying physical states, not merely a statement that experimental preparation choices are independent. The excluded [psi-epistemic model](../../../../../psi-epistemic-model.md) hypothesis is that the same physical state can occur with positive probability for two different pure-state preparations. The theorem neither excludes additional hidden variables nor claims that every interpretation which speaks of information is ruled out without these assumptions.

For the two given [qubit](../../../../../qubit.md) preparations, consider the following [PBR exclusion measurement for zero and plus](../../../../../pbr-exclusion-measurement-for-zero-and-plus.md), written in the ordered basis $00,01,10,11$:

$$
\begin{aligned}
|\xi_{00}\rangle&=(|01\rangle+|10\rangle)/\sqrt2,\\
|\xi_{0+}\rangle&=(|00\rangle-|01\rangle+|10\rangle+|11\rangle)/2,\\
|\xi_{+0}\rangle&=(|00\rangle+|01\rangle-|10\rangle+|11\rangle)/2,\\
|\xi_{++}\rangle&=(|00\rangle-|11\rangle)/\sqrt2.
\end{aligned}
$$

Direct [inner products](../../../../../inner-product.md) show that these four vectors are an [orthonormal basis](../../../../../orthonormal-basis.md). Each labelled vector is orthogonal to the correspondingly labelled product preparation, so the associated [projective measurement](../../../../../projective-measurement.md) satisfies

$$
\boxed{\Pr(xy\mid|x\rangle|y\rangle)=|\langle\xi_{xy}|x,y\rangle|^2=0,\qquad x,y\in\{0,+\}.}
$$

This is an example of [antidistinguishable quantum states](../../../../../antidistinguishable-quantum-states.md): every outcome excludes one possible preparation, although the preparations cannot be perfectly distinguished.

To prove the contradiction without requiring deterministic [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) responses, choose a common dominating measure for $\mu_0,\mu_+$ and write their densities $m_0,m_+$. If they overlap, $\nu(\lambda)=\min(m_0,m_+)$ has mass $\varepsilon>0$. By [preparation independence](../../../../../preparation-independence.md), every one of the four product densities dominates $\nu(\lambda_1)\nu(\lambda_2)$. Its total mass is $\varepsilon^2$. The zero [Born rule](../../../../../born-rule.md) probability for outcome $xy$ implies that its nonnegative response $\xi_{xy}(\lambda_1,\lambda_2)$ vanishes almost everywhere for its matching preparation, hence also under this common product measure. All four responses would then vanish on a set of positive measure, contradicting their sum being one. Therefore **$\mu_0$ and $\mu_+$ are mutually singular**.

For the second pair, group the $2n$ independent preparations into two blocks of $n$. Define $|\Psi_i\rangle=|\psi_i\rangle^{\otimes n}$. The [tensor-power reduction of PBR overlap](../../../../../tensor-power-reduction-of-pbr-overlap.md) gives

$$
\langle\Psi_1|\Psi_2\rangle=\langle\psi_1|\psi_2\rangle^n=1/\sqrt2.
$$

Each block therefore has an effective two-dimensional [Hilbert space](../../../../../hilbert-space-split.md). Explicitly,

$$
|e_0\rangle=|\Psi_1\rangle,\qquad
|e_1\rangle=\sqrt2|\Psi_2\rangle-|\Psi_1\rangle
$$

are orthonormal and $|\Psi_2\rangle=(|e_0\rangle+|e_1\rangle)/\sqrt2$. Embed the four-vector exclusion basis above into the [tensor product](../../../../../tensor-product.md) of these two block spaces. To obtain a complete [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) on all $2n$ [qubits](../../../../../qubit.md), add the orthogonal complement of that four-dimensional subspace to one of its four projectors. All four allowed preparations lie in the subspace, so the four forbidden probabilities remain zero.

If the single-copy preparation distributions overlap with common mass $\varepsilon>0$, their $2n$-fold products all dominate the common measure $\nu^{\otimes2n}$ of mass $\varepsilon^{2n}>0$. The same zero-response contradiction now applies to the four block preparations. Thus

$$
\boxed{\mu_{\psi_1}\perp\mu_{\psi_2}.}
$$

The argument is exact for the ideal devices specified in the question; no finite experimental resolution or noisy overlap bound is assumed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
