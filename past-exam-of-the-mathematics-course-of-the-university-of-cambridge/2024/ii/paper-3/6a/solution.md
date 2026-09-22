<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

The transition rates of this [birth-death process](../../../../../birth-death-process.md) are $q_{n,n+1}=\lambda n$ and $q_{n,n-1}=n(\gamma+\beta n)$. Thus, with $p_{-1}=0$,

$$
\dot p_n=\lambda(n-1)p_{n-1}+(n+1)(\gamma+\beta(n+1))p_{n+1}
-[\lambda n+n(\gamma+\beta n)]p_n.
$$

Multiplying by $n$, summing, and shifting indices gives

$$
\frac d{dt}\mathbb E N=(\lambda-\gamma)\mathbb EN-\beta\mathbb E(N^2).
$$

At a finite-moment steady state with positive mean and $\lambda>\gamma$,

$$
\beta\mathbb E(N^2)=(\lambda-\gamma)\mathbb EN.
$$

Since $\mathbb E(N^2)\geq(\mathbb EN)^2$, this implies

$$
0<\mathbb EN\leq\frac{\lambda-\gamma}{\beta}.
$$

If $\lambda\leq\gamma$, both terms in the mean equation are nonpositive, and stationarity forces $\mathbb EN=0$. Thus the population is extinct almost surely in any such steady state.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
