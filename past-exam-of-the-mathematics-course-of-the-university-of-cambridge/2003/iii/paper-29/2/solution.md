<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A convenient precise version is the [almost sure submartingale convergence theorem](../../../../../almost-sure-submartingale-convergence-theorem.md): if $(S_n)$ is a real [submartingale](../../../../../submartingale.md) and $\sup_n\mathbb E S_n^+<\infty$, then $S_n$ converges [almost surely](../../../../../almost-sure-convergence.md) to a finite [integrable random variable](../../../../../integrable-random-variable.md). In particular the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) applies to any [martingale](../../../../../martingale-split.md) with $\sup_n\mathbb E|S_n|<\infty$. It asserts neither [convergence in L1](../../../../../convergence-in-l1.md) nor preservation of the initial [expected value](../../../../../expected-value.md) without additional [uniform integrability](../../../../../uniform-integrability.md).

Here is a proof including the crossing estimate. Fix real $a<b$, and let $U_n[a,b]$ count completed [upcrossings](../../../../../upcrossing.md) by time $n$. Use a predictable indicator $H_k$ which holds one unit during each crossing attempt: enter when $S_k\leq a$, exit when $S_k\geq b$. With

$$
G_n=\sum_{k=0}^{n-1}H_k(S_{k+1}-S_k),
$$

each completed trade gains at least $b-a$, while the possible unfinished trade loses no more than $(S_n-a)^-$. Hence $G_n\geq(b-a)U_n[a,b]-(S_n-a)^-$. The [submartingale](../../../../../submartingale.md) property and $0\leq H_k\leq1$ give $\mathbb E G_n\leq\mathbb E(S_n-S_0)$: the complementary predictable gains have nonnegative [expected value](../../../../../expected-value.md). Therefore

$$
(b-a)\mathbb E U_n[a,b]\leq\mathbb E(S_n-S_0)+\mathbb E(S_n-a)^-=\mathbb E(S_n-a)^++a-\mathbb E S_0.
$$

The right side is uniformly bounded, since $(S_n-a)^+\leq S_n^++|a|$. By the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), every rational interval has finitely many [upcrossings](../../../../../upcrossing.md) [almost surely](../../../../../almost-sure-convergence.md). A real sequence whose lower and upper limits differ crosses some rational interval infinitely often, so the [countable](../../../../../countable-set.md) intersection of these events gives an extended-real limit. Furthermore

$$
\mathbb E S_n^- =\mathbb E S_n^+-\mathbb E S_n\leq\sup_m\mathbb E S_m^+-\mathbb E S_0,
$$

so $\sup_n\mathbb E|S_n|<\infty$. The [Fatou lemma](../../../../../fatou-s-lemma.md) makes the limit finite and [integrable](../../../../../integrability.md), completing the proof. Applying this theorem to $-Z_n$ gives the [almost sure supermartingale convergence theorem](../../../../../almost-sure-supermartingale-convergence-theorem.md) for nonnegative [supermartingales](../../../../../supermartingale.md).

For the given adapted multiplicative drift, put

$$
P_0=1,\qquad P_n=\prod_{k=0}^{n-1}(1+Y_k),\qquad Z_n=\frac{X_n}{P_n}.
$$

The next denominator $P_{n+1}$ is $\mathcal F_n$-[measurable](../../../../../measurability.md), and $P_n\geq1$ makes $Z_n$ [integrable](../../../../../integrability.md). Thus

$$
\mathbb E[Z_{n+1}\mid\mathcal F_n]=\frac{\mathbb E[X_{n+1}\mid\mathcal F_n]}{P_{n+1}}\leq\frac{(1+Y_n)X_n}{P_{n+1}}=Z_n.
$$

The nonnegative [supermartingale](../../../../../supermartingale.md) $Z_n$ has a finite [almost sure convergence](../../../../../almost-sure-convergence.md) limit $Z_\infty$. On the probability-one event where the specified series is finite,

$$
0\leq\log P_n=\sum_{k<n}\log(1+Y_k)\leq\sum_{k\geq0}Y_k<\infty.
$$

Consequently $P_n\uparrow P_\infty\in[1,\infty)$ and the [multiplicative correction for summable adapted drift](../../../../../multiplicative-correction-for-summable-adapted-drift.md) gives

$$
\boxed{X_n\longrightarrow P_\infty Z_\infty<\infty\quad\text{almost surely}.}
$$

The argument does not require a finite [expected value](../../../../../expected-value.md) for the infinite product or for the total drift.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
