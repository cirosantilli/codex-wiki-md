<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Within the active set, cross-classify dosage $Z_i\in\{1,2\}$ against $Y_i$. Conditional on the vector $A=(A_1,\ldots,A_n)$, complete randomization assigns $n_1$ of the active patients to low dosage and $n_2$ to high dosage uniformly. Under independent assignment, active patients receive low and high dosage with conditional probabilities

$$
\frac{\pi_1}{\pi_1+\pi_2}
\quad\text{and}\quad
\frac{\pi_2}{\pi_1+\pi_2};
$$

conditioning further on their low- and high-dose totals again gives the same uniform allocation. Under $H_B$, active patients' outcomes are fixed as their common $Y_i(1)=Y_i(2)$, so the conditional Fisher p-value obeys

$$
\mathbb P(P_B\leq\alpha_2\mid A)\leq\alpha_2.
$$

Under $H_A$, $P_A$ is a function only of $A$ and the fixed outcomes. Applying the [law of iterated expectation](../../../../../../law-of-total-expectation.md) under the joint null gives

$$
\begin{aligned}
\mathbb P(P_A\leq\alpha_1,P_B\leq\alpha_2)
&=\mathbb E\!\left[
\mathbf1_{\{P_A\leq\alpha_1\}}
\mathbb P(P_B\leq\alpha_2\mid A)
\right]\\
&\leq\alpha_2\mathbb P(P_A\leq\alpha_1)
\leq\alpha_1\alpha_2.
\end{aligned}
$$

This conditional argument explains the stated near-independence even though the two tests reuse outcomes.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
