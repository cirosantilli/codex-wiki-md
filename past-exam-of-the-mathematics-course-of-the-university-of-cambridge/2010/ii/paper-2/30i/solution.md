<h1 id="30i/solution">Solution</h1>

↑ **Parent:** [30I](../30i.md)

Relative to a [filtration](../../../../../filtration-probability-theory.md) $(\mathcal F_n)$, a [martingale](../../../../../martingale-split.md) is an adapted integrable process with $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$; a [supermartingale](../../../../../supermartingale.md) has the corresponding inequality $\leq$. A [stopping time](../../../../../stopping-time.md) $T$ has $\{T\leq n\}\in\mathcal F_n$ for every $n$.

For $T\leq N$, the pathwise identity

$$
M_T=M_0+\sum_{k=1}^N\mathbf1_{\{T\geq k\}}(M_k-M_{k-1})
$$

has $\mathcal F_{k-1}$-measurable indicators. Conditioning each summand gives zero expected increment for a [martingale](../../../../../martingale-split.md), and a nonpositive one for a [supermartingale](../../../../../supermartingale.md). All terms are integrable because the sum is finite. Thus $\mathbb EM_T=\mathbb EM_0$ and $\mathbb E\hat M_T\leq\mathbb E\hat M_0$, proving the requested inequality when their initial values agree.

A [self-financing strategy](../../../../../self-financing-portfolio.md) holds $\pi_n$ shares during period $n$, chosen using information at time $n-1$. Its cash investment is $X_{n-1}-\pi_nS_{n-1}$, which earns the risk-free return. Hence

$$
X_n=\pi_nS_n+(1+r)(X_{n-1}-\pi_nS_{n-1})
=(1+r)X_{n-1}+\pi_n[S_n-(1+r)S_{n-1}].
$$

Use the terminal condition $V(N,x,s)=U(x)$ from the original PDF. Conditional on the current state and past, the next return has the law of $\xi_1$ and is independent of the past. Therefore the conditional expectation of $V(n+1,X_{n+1},S_{n+1})$ for the chosen holding $\pi_{n+1}$ is at most its supremum over all holdings, namely $V(n,X_n,S_n)$. Assuming the finite values and integrability implicit in this stochastic-control formulation, the value process is a [supermartingale](../../../../../supermartingale.md).

It follows that $\mathbb E U(X_N)\leq V(0,X_0,S_0)$ for every admissible strategy. If the strategy $\pi^*$ makes this process a [martingale](../../../../../martingale-split.md), equality holds for it. **$\pi^*$ attains the upper bound and is optimal.** No existence of an optimizer or finiteness of an unconstrained supremum is being assumed without the stated admissibility conditions.

## ↑ Ancestors (10)

1. [30I](../30i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
