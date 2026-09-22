<h1 id="4/i/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Conjugation by a [Pauli operator](../../../../../../../pauli-operator.md) preserves its matching [Bloch vector](../../../../../../../bloch-vector.md) component and reverses the other two. Summing all three conjugations therefore sends $\mathbf s$ to $-\mathbf s$. The specified [quantum depolarizing channel](../../../../../../../quantum-depolarizing-channel.md) has retention factor

$$
\eta=p-\frac{1-p}{3}=\frac{4p-1}{3},\qquad
\mathbf s\longmapsto\eta\mathbf s.
$$

This [Pauli-mixture parametrization of qubit depolarization](../../../../../../../pauli-mixture-parametrization-of-qubit-depolarization.md) differs from a convention in which $p$ itself is the retention factor. For $0\leq p\leq1$, $-1/3\leq\eta\leq1$. A pure input gives output eigenvalues $(1\pm|\eta|)/2$, and hence entropy $h_2((1+\eta)/2)$ by symmetry of [binary entropy](../../../../../../../binary-entropy.md). Mixed inputs have a smaller output radius and at least this much entropy. Every average output has entropy at most one. Thus

$$
\chi(\mathcal E_{\rm out})\leq1-h_2\left(\frac{1+\eta}{2}\right).
$$

Two equiprobable orthogonal pure inputs have antipodal output [Bloch vectors](../../../../../../../bloch-vector.md), maximally mixed average output, and this same minimal individual output entropy. They attain the bound. Applying the coding theorem gives

$$
\boxed{C_{\rm prod}(\Lambda)=1-h_2\left(\frac{2p+1}{3}\right)
\quad\text{bits per channel use}.}
$$

At $p=1$ it is one; at $p=1/4$ it is zero; at $p=0$ it is $1-h_2(1/3)\simeq0.0817$. Negative retention reverses the labels of the two signals but does not eliminate their distinguishability.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [I](../../i.md)
3. [4](../../../4.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
