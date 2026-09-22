<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is now no separate rate-$\nu$ clockwise transition. The only transitions are

$$
(m,n)\longrightarrow(m-1,n+1)\quad\text{at rate }\lambda_m,
\qquad
(m,n)\longrightarrow(m+1,n-1)\quad\text{at rate }\mu\quad(n>0).
$$

Both preserve $m+n$ modulo $M$. The initial state therefore selects the [closed communicating class](../../../../../../closed-communicating-class.md) $m+n\equiv0\pmod M$, on which $m\equiv-n\pmod M$. The population is a [birth-death process](../../../../../../birth-death-process.md) with birth rate $\lambda_{-n}$ and death rate $\mu$.

Define $a_0=1$ and $a_r=\mu^{-r}\prod_{j=0}^{r-1}\lambda_{-j}$ for $1\leq r<M$. The [detailed balance for a birth-death process](../../../../../../detailed-balance-for-a-birth-death-process.md) weights are

$$
w_n=\mu^{-n}\prod_{j=0}^{n-1}\lambda_{-j}.
$$

Writing $n=kM+r$ with $0\leq r<M$, the product condition gives $w_n=a_r\rho^{kM}$. Summing the resulting [geometric series](../../../../../../geometric-series.md) yields

$$
\boxed{\pi(m,kM+r)=\mathbf1_{\{m+r\equiv0\pmod M\}}\frac{(1-\rho^M)a_r\rho^{kM}}{\sum_{s=0}^{M-1}a_s}.}
$$

This is also the law in part (b) conditioned on $m+n\equiv0\pmod M$: the ratio of its weights at consecutive accessible populations is $\lambda_{-n}/\mu$. The stability condition is $\mu>\nu$, which uses the product of the periodic birth rates; it does not require $\mu>\lambda_m$ for every $m$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
