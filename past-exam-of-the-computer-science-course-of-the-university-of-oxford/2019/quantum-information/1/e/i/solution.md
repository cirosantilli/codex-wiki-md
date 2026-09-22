<h1 id="1/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\delta=\pi/(2n)$. Between successive measurement bases, the squared overlap is $c=\cos^2\delta$ for retaining the same label and $s=\sin^2\delta$ for changing label. The first step obeys the same rule if we regard the initial state as label 0 at angle zero. Thus the recorded labels form a [Markov chain](../../../../../../markov-chain-split.md) with [transition matrix](../../../../../../stochastic-matrix.md) $\bigl(\begin{smallmatrix}c&s\\s&c\end{smallmatrix}\bigr)$.

Let $q_k$ be the [probability](../../../../../../probability.md) of label 0 after step $k$. Then $q_0=1$ and

$$
q_k=cq_{k-1}+s(1-q_{k-1}),\qquad 2q_k-1=(c-s)(2q_{k-1}-1).
$$

Since $c-s=\cos(\pi/n)$, iteration yields

$$
\boxed{q_n=\frac12\left[1+\cos^n\left(\frac\pi n\right)\right].}
$$

This is the total final-outcome [probability](../../../../../../probability.md), including histories that change label an [even number](../../../../../../even-number.md) of times. The smaller quantity $\cos^{2n}(\pi/(2n))$ counts only the history with label 0 at every step and is not the requested total. For example, at $n=3$ the total is $9/16$, whereas the uninterrupted history has [probability](../../../../../../probability.md) $27/64$. At $n=1$, the final basis is $\{|1\rangle,|0\rangle\}$ up to signs, so the total [probability](../../../../../../probability.md) of label 0 is zero, as the formula also gives. This distinguishes nonselective [measurement-guided Zeno transfer](../../../../../../measurement-guided-zeno-transfer.md) from [postselection](../../../../../../postselection.md) on one record.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
