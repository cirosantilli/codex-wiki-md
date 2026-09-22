<h1 id="n/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Starting from a state $i$, let $\tau_i=\inf\{n\ge1:X_n=i\}$ be the [first return time](../../../../../first-return-time.md), with value infinity if no return occurs. The state is recurrent if $\Pr_i(\tau_i<\infty)=1$ and transient if this [probability](../../../../../probability.md) is less than 1. A [recurrent state](../../../../../recurrent-state.md) is [positive recurrent](../../../../../positive-recurrent-markov-chain.md) if $\mathbb E_i\tau_i<\infty$, and [null recurrent](../../../../../null-recurrent-state.md) if that [expectation](../../../../../expected-value-split.md) is infinite.

If $i$ and $j$ communicate, choose $r,s$ with $p_{ij}^{(r)}>0$ and $p_{ji}^{(s)}>0$. The [Chapman-Kolmogorov equations](../../../../../chapman-kolmogorov-equation.md) give, for every $n$,

$$
p_{ii}^{(r+n+s)}\ge p_{ij}^{(r)}p_{jj}^{(n)}p_{ji}^{(s)}.
$$

If $j$ is recurrent, the supplied criterion makes $\sum_n p_{jj}^{(n)}$ infinite. Summing this inequality shows that $\sum_n p_{ii}^{(n)}$ is also infinite, so $i$ is recurrent. The same argument with the states exchanged gives the converse. Hence **recurrence and transience are class properties**: states in one [communicating class](../../../../../communicating-class.md) cannot have different answers to that dichotomy.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [N](../../../n.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
