<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [stationary balance equations](../../../../../../global-balance-for-a-continuous-time-markov-chain.md) at level zero are $(\lambda+\alpha)\pi_{0C}=\beta\pi_{0W}$ and $\beta\pi_{0W}=\alpha\pi_{0C}+\mu\pi_{1W}$. At every $i\geq1$ they are

$$
(\lambda+\alpha)\pi_{iC}=\lambda\pi_{i-1,C}+\beta\pi_{iW},\qquad
(\mu+\beta)\pi_{iW}=\alpha\pi_{iC}+\mu\pi_{i+1,W}.
$$

The zero-level equations give $\pi_{0C}=\beta\pi_{0W}/(\lambda+\alpha)$ and $\pi_{1W}=\beta\lambda\pi_{0W}/[\mu(\lambda+\alpha)]$. Substituting the latter in the level-one $C$ equation gives

$$
(\pi_{1C},\pi_{1W})=\frac{\beta\pi_{0W}}{\lambda+\alpha}\left(\frac{\lambda(\mu+\beta)}{\mu(\lambda+\alpha)},\frac\lambda\mu\right).
$$

Solve the $W$ equation for $\pi_{i+1,W}$, then substitute it into the next $C$ equation. This yields the required row-vector recurrence with

$$
\boxed{B=\begin{pmatrix}\frac{\lambda\mu-\beta\alpha}{\mu(\lambda+\alpha)}&-\frac\alpha\mu\\\frac{\beta(\beta+\mu)}{\mu(\lambda+\alpha)}&\frac{\beta+\mu}\mu\end{pmatrix}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
