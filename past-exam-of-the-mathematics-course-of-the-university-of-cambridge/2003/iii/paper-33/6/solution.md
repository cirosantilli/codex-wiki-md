<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $(A_t,B_t)$ be a [Markov jump process](../../../../../markov-jump-process.md) on integer populations, with rates

$$
(a,b)\longrightarrow(a-1,b)\text{ at rate }\kappa b,\qquad(a,b)\longrightarrow(a,b-1)\text{ at rate }\kappa a
$$

when $a,b>0$, where $\kappa>0$. Make both axes absorbing, so the fight ends when one population reaches zero. Start at $(N,b_N)$, with $b_N=\lfloor\alpha N\rfloor$; when $\alpha N$ is integral this is the printed initial condition exactly. The harmless rounding convention makes the model defined for every integer $N$.

Use the embedded [jump chain](../../../../../jump-chain.md) $(A_j,B_j)$ rather than physical time. Its probabilities of the two losses are respectively $b/(a+b)$ and $a/(a+b)$, independently of $\kappa$. It reaches an axis after at most $N+b_N\leq2N$ steps; hold it constant thereafter. Put

$$
D_j=A_j^2-B_j^2.
$$

Before absorption its two increments are $-2a+1$ and $2b-1$, so

$$
\mu_j=\mathbb E[D_j-D_{j-1}\mid\mathcal F_{j-1}]=\frac{b-a}{a+b},\qquad |\mu_j|\leq1.
$$

After absorption set $\mu_j=0$. Consequently

$$
M_j=D_j-D_0-\sum_{r=1}^j\mu_r
$$

is a discrete-time [martingale](../../../../../martingale-split.md). All populations are at most $N$, so each martingale difference is bounded in absolute value by $2N+2\leq4N$. The total drift up to step $2N$ is at most $2N$. This is the [squared-population near-invariant for stochastic attrition](../../../../../squared-population-near-invariant-for-stochastic-attrition.md).

The two-sided [Azuma-Hoeffding inequality](../../../../../azuma-s-inequality.md) states that a martingale with $m$ differences bounded by $C$ satisfies $\mathbb P(|M_m|\geq z)\leq2\exp(-z^2/(2mC^2))$. Its exponential estimate follows by applying the conditional [Hoeffding lemma](../../../../../hoeffding-lemma.md) to each centered difference, iterating, and optimizing the exponential Markov bound. With $m=2N$ and $C=4N$ it gives

$$
\mathbb P(|M_{2N}|\geq\eta N^2)\leq2\exp(-\eta^2N/64).
$$

Let $c=\sqrt{1-\alpha^2}>0$, and let $X^N=A_{2N}/N$ be the final proportion. If the first population survives, then the second is zero and $D_{2N}/N^2=(X^N)^2$. Hence $|X^N-c|>\delta$ implies

$$
|D_{2N}-c^2N^2|=N^2|X^N-c|(X^N+c)>c\delta N^2.
$$

If the first population is extinguished, $X^N=0$ and $D_{2N}\leq0$. This can satisfy the indicated deviation event only when $\delta<c$, and then $|D_{2N}-c^2N^2|\geq c^2N^2>c\delta N^2$. Thus the same implication holds in both cases.

The initial rounding error obeys $|D_0-c^2N^2|=|\alpha^2N^2-b_N^2|\leq2N$. Combining it with the drift bound shows that the deviation event forces

$$
|M_{2N}|>c\delta N^2-4N\geq\tfrac12c\delta N^2
$$

for all sufficiently large $N$. Set $\eta=c\delta/2$ in the preceding concentration inequality. We conclude

$$
\boxed{\mathbb P(|X^N-\sqrt{1-\alpha^2}|>\delta)\leq2e^{-(1-\alpha^2)\delta^2N/256}}
$$

for sufficiently large $N$, and therefore

$$
\boxed{\limsup_{N\to\infty}\frac1N\log\mathbb P(|X^N-\sqrt{1-\alpha^2}|>\delta)\leq-\frac{(1-\alpha^2)\delta^2}{256}<0.}
$$

The [symmetric stochastic attrition process](../../../../../symmetric-stochastic-attrition-process.md) thus has [exponential concentration of terminal stochastic attrition survivors](../../../../../exponential-concentration-of-terminal-stochastic-attrition-survivors.md). The deterministic equations conserve $a^2-b^2$ and predict the same surviving fraction, but the martingale argument supplies the stronger exponential probability estimate required here.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
