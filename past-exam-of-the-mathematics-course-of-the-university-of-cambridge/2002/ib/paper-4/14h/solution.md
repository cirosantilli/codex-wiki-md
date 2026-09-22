<h1 id="14h/solution">Solution</h1>

↑ **Parent:** [14H](../14h.md)

First take $s_i>0$, the hypothesis required for the printed ratios and their optimization formula to be well-defined. Since $\sum p_i=1$,

$$
\sum_i\frac{p_ix_i}{s_i+x_i}=1-\sum_i\frac{p_is_i}{s_i+x_i}.
$$

The maximizing and minimizing problems therefore have exactly the same solutions.

Let $\tau>0$ and minimize the separable [optimization Lagrangian](../../../../../optimization-lagrangian.md)

$$
L(x,\tau)=\sum_i\frac{p_is_i}{s_i+x_i}+\tau\left(\sum_i x_i-b\right),\qquad x_i\ge0.
$$

Each summand is convex, and its [derivative](../../../../../derivative.md) is $-p_is_i/(s_i+x_i)^2+\tau$. Its minimizer is $x_i(\tau)=(\sqrt{p_is_i/\tau}-s_i)^+$. The sum of these coordinates is continuous in $\tau$, decreases from infinity to zero, and is strictly decreasing wherever positive. Thus there is a unique $\tau$ for which the sum is $b$. For every feasible $y$, coordinatewise minimization gives $L(y,\tau)\ge L(x(\tau),\tau)$; both constraint terms vanish. The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) proves global optimality, not just a necessary stationary condition.

Put $r_i=p_i/s_i$ in decreasing order. A positive bet occurs exactly when $r_i>\tau$. Hence the positive bets form an initial block. To interpret the maximal index in the question, one may include any subsequent indices tied at $r_i=\tau$: their bets are zero but their marginal-return equality still holds. Take $k=\max\{i:r_i\ge\tau\}$. Then

$$
\boxed{\frac{p_1s_1}{(s_1+x_1)^2}=\cdots=\frac{p_ks_k}{(s_k+x_k)^2}=\tau,\qquad x_i=0\ (i>k).}
$$

For this block, $\sqrt\tau=(\sum_{i\le k}\sqrt{p_is_i})/(b+\sum_{i\le k}s_i)$, with the threshold inequalities determining $k$. Zero-[probability](../../../../../probability.md) horses receive zero bets.

Let $H$ be the set attaining $\rho=\max r_i$, and write $S_H=\sum_{i\in H}s_i$, $P_H=\sum_{i\in H}p_i=\rho S_H$. For sufficiently small $b$, the solution uses only $H$, with $x_i=bs_i/S_H$ there and $\tau=\rho[S_H/(S_H+b)]^2$. If the next ratio is $r_*<\rho$, this remains valid when $b\le S_H(\sqrt{\rho/r_*}-1)$; if all outside ratios are zero there is no finite threshold. Put $S=\sum_i s_i$. The fixed pool is $S+b$, so the expected gross payout and net gain are

$$
\boxed{E(\text{payout})=(S+b)\frac{P_Hb}{S_H+b},\qquad E(\text{net gain})=(S+b)\frac{P_Hb}{S_H+b}-b.}
$$

Tied best horses receive bets proportional to their existing stakes; betting all on one tied horse is not generally optimal for finite $b$. This is [pari-mutuel expected-return allocation](../../../../../pari-mutuel-expected-return-allocation.md).

The literal allowance $s_i=0$ needs qualification. At $s_i=x_i=0$ the printed objective contains $0/0$ and the ordered ratios are undefined. Even defining an unbacked horse's payout to be zero does not always yield an attained optimum. For example, take $b=1$, $p_1=p_2=1/2$, $s_1=0$, $s_2=1$. For $x_1>0$, the normalized expected payout is $1/2+(1/2)(1-x_1)/(2-x_1)$, tending to $3/4$ as $x_1\downarrow0$ but never attaining it; at $x_1=0$ that zero-payout convention gives $1/4$. Thus **the proved allocation formula requires positive existing stakes, or an explicitly modified market model**. The zero-stake case cannot be justified by silently dividing by zero.

## ↑ Ancestors (10)

1. [14H](../14h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
