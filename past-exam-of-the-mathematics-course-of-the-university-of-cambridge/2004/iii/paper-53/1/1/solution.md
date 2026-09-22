<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Apply the [Born rule](../../../../../../born-rule.md) to the two amplitudes in the introductory calculation. In the [computational basis](../../../../../../computational-basis.md), the probabilities are

$$
\boxed{P_0(\phi)=\frac{1+\cos\phi}{2},\qquad P_1(\phi)=\frac{1-\cos\phi}{2}.}
$$

The other basis printed in this question is $(|0\rangle\pm i|1\rangle)/\sqrt2$, the [Pauli Y gate](../../../../../../pauli-y-gate.md) eigenbasis. It is not the real [Hadamard basis](../../../../../../hadamard-basis.md). Write the output amplitudes as $a=(1+e^{i\phi})/2$ and $b=(1-e^{i\phi})/2$. The plus-outcome amplitude is $(a-ib)/\sqrt2$ and the minus-outcome amplitude is $(a+ib)/\sqrt2$. Since $\operatorname{Im}(\overline a b)=-\sin\phi/2$, the [Born rule](../../../../../../born-rule.md) gives

$$
\boxed{P_+(\phi)=\frac{1-\sin\phi}{2},\qquad P_-(\phi)=\frac{1+\sin\phi}{2}.}
$$

In particular, at $\phi=\pi/2$ the output is the minus eigenstate, which checks the sign of the imaginary quadrature.

Use separate fresh runs for each measurement basis. If $\widehat P_j$ denotes the empirical outcome frequency, then

$$
\boxed{\widehat{\langle u|U|u\rangle}=(\widehat P_0-\widehat P_1)+i(\widehat P_--\widehat P_+).}
$$

The two differences estimate $\cos\phi$ and $\sin\phi$, resolving the ambiguity that would remain from the first basis alone. Each [Bernoulli](../../../../../../bernoulli-distribution.md) frequency converges by the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md), with standard error of order the inverse square root of the number of runs. One may project the noisy estimate onto the unit circle if a phase estimate is desired, but that projection is not necessary for consistency.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
