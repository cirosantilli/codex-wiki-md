<h1 id="m/m5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $Q=\sum_{m=1}^N1/m$ and propose $\pi_N=1/Q$, $\pi_j=1/((j+1)Q)$ for $j<N$. These probabilities sum to one because $1+\sum_{j=1}^{N-1}1/(j+1)=Q$.

For $j<N$, the incoming stationary [probability](../../../../../../probability.md) is

$$
\sum_{k=j+1}^N\frac{\pi_k}{k}
=\frac1Q\left\{\sum_{k=j+1}^{N-1}\frac1{k(k+1)}+\frac1N\right\}
=\frac1{(j+1)Q}=\pi_j,
$$

using the telescoping identity $1/(k(k+1))=1/k-1/(k+1)$. Similarly $\sum_{k=1}^N\pi_k/k=1/Q=\pi_N$. Thus $\pi$ is stationary.

The finite chain is irreducible: every state can reach $N$, and from $N$ every state is reachable in one step. Its self-loop at $N$ makes it aperiodic. The finite-state convergence theorem therefore gives the claimed limit from any initial state:

$$
\boxed{\lim_{n\to\infty}\Pr(X_n=j)=\begin{cases}1/((j+1)Q),&1\leq j<N,\\1/Q,&j=N.\end{cases}}
$$

For $N=1$ this is the single absorbing refill state and the same formula gives [probability](../../../../../../probability.md) one.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
