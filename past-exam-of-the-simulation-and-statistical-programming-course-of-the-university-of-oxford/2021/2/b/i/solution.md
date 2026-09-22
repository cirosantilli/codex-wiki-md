<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because $U\in[0,1]$, the conditional acceptance [probability](../../../../../probability.md) is $a_k=\min(1,\lambda^k)$, even when the printed threshold exceeds one. Repeating rejected trials gives the [clipped acceptance reweighting identity](../../../../../clipped-acceptance-reweighting-identity.md):

$$
\mathbb P(X=k)=\frac{e^{-\lambda}\lambda^k a_k/k!}{\sum_{j\geq0}e^{-\lambda}\lambda^j a_j/j!}.
$$

For $0<\lambda<1$, $a_k=\lambda^k$, including $a_0=1$. The denominator is $e^{-\lambda}\sum_k\lambda^{2k}/k!=e^{\lambda^2-\lambda}$, so

$$
\boxed{X\sim
\begin{cases}
\operatorname{Poisson}(\lambda^2),&0<\lambda<1,\\
\operatorname{Poisson}(\lambda),&\lambda\geq1.
\end{cases}}
$$

For $\lambda\geq1$ every proposal is accepted, so reweighting by $\lambda^k$ would be incorrect. At $\lambda=1$ both formulas agree. Termination has [probability](../../../../../probability.md) one since the acceptance [probability](../../../../../probability.md) is $e^{\lambda^2-\lambda}>0$ in the first case and one in the second.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
