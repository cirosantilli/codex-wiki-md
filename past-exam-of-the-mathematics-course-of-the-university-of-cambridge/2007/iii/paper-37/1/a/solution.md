<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the compartment counts $Z_n=(S_n,I_n,R_n)$ as the state of the [SIRS Markov chain](../../../../../../sirs-markov-chain.md). Its state space is $\{(S,I,R)\in\mathbb Z_{\ge0}^3:S+I+R=n\}$. The [transition rates](../../../../../../transition-intensity.md) are

$$
\begin{array}{c|c}
\text{new state}&\text{rate from }(S,I,R)\\\hline
(S-1,I+1,R)&\lambda SI/n\\
(S,I-1,R+1)&\gamma I\\
(S+1,I,R-1)&\nu R.
\end{array}
$$

Each susceptible has infection hazard $\lambda I/n$, so summing over the $S$ susceptibles gives the first rate. The [memorylessness of the exponential distribution](../../../../../../memorylessness-of-the-exponential-distribution.md) makes each of the $I$ current infectives have recovery hazard $\gamma$, irrespective of its infection time. Each removed individual has immunity-loss hazard $\nu$. These are all the possible off-diagonal transitions. The diagonal entry of the [transition intensity matrix](../../../../../../transition-intensity-matrix.md) is minus their sum, and a transition with no eligible individual has rate zero. Thus **the three total event rates are $\lambda SI/n$, $\gamma I$ and $\nu R$**, and every event conserves population size.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
