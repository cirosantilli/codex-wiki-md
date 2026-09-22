<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write

$$
R_{M,N}=\frac{S_N}{S_M}
$$

for the product of the last $N-M$ stock factors. The forward-start payoff is

$$
(S_N-\lambda S_M)^+
=S_M(R_{M,N}-\lambda)^+.
$$

Under the risk-neutral measure the binomial factors are independent with the same probability $q$ at every node. Hence $S_M$ and $R_{M,N}$ are independent, while

$$
\mathbb E_QS_M=S_0(1+r)^M.
$$

The [forward-start call option](../../../../../../forward-start-call-option.md) consequently has price

$$
\begin{aligned}
\operatorname{FSC}(M,N,\lambda)
&=(1+r)^{-N}\mathbb E_Q
\left[S_M(R_{M,N}-\lambda)^+\right]\\
&=S_0(1+r)^{-(N-M)}
\mathbb E_Q\left[(R_{M,N}-\lambda)^+\right].
\end{aligned}
$$

An ordinary $(N-M)$-period call with strike $K$ has price

$$
\operatorname{EC}(N-M,K)
=S_0(1+r)^{-(N-M)}
\mathbb E_Q\left[\left(R_{M,N}-\frac K{S_0}\right)^+\right].
$$

The required equality therefore holds for

$$
\boxed{K=\lambda S_0}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
