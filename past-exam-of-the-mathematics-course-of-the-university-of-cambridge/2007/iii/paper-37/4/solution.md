<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The exponent printed in the original PDF is too strong under the stated increment bound. Take $M_0=0$, let $M_1$ equal $1$ or $-1$ with equal probabilities, and set $M_k=M_1$ for $k\ge1$. This is a [martingale](../../../../../martingale-split.md) with $c_1=1$ and $c_k=0$ for $k>1$. For $n=1$ and $x=1$,

$$
\mathbb P(|M_1-M_0|\ge1)=1>2e^{-1}.
$$

Thus **the printed inequality is false**. The intended [two-sided Azuma-Hoeffding inequality](../../../../../two-sided-azuma-hoeffding-inequality.md) is

$$
\boxed{\mathbb P(|M_n-M_0|\ge x)
\le2\exp\left(-\frac{x^2}{2\sum_{k=1}^nc_k^2}\right).}
$$

Here the $c_k$ are deterministic increment bounds. We prove this corrected assertion from conditional exponential moments.

Let $D_k=M_k-M_{k-1}$. The [martingale](../../../../../martingale-split.md) property gives $\mathbb E[D_k\mid\mathcal F_{k-1}]=0$. For $c_k>0$, convexity of the [exponential function](../../../../../exponential-function.md) gives the secant bound on $[-c_k,c_k]$,

$$
e^{\theta D_k}\le\frac{c_k+D_k}{2c_k}e^{\theta c_k}
+\frac{c_k-D_k}{2c_k}e^{-\theta c_k}.
$$

Taking [conditional expectation](../../../../../conditional-expectation.md) removes the terms containing $D_k$, so

$$
\mathbb E[e^{\theta D_k}\mid\mathcal F_{k-1}]
\le\cosh(\theta c_k)\le e^{\theta^2c_k^2/2}.
$$

The last inequality follows term by term from $(2j)!\ge2^jj!$ in the power series for $\cosh z$ and $e^{z^2/2}$. If $c_k=0$ the increment is zero and the same bound holds directly. This is the bounded-increment case of the [Hoeffding lemma](../../../../../hoeffding-lemma.md).

Repeated conditioning, without any [independence](../../../../../independent-random-variables.md) assumption, now gives

$$
\mathbb E\exp\bigl(\theta(M_n-M_0)\bigr)
\le\exp\left(\frac{\theta^2}2\sum_{k=1}^nc_k^2\right).
$$

Write $C=\sum_{k=1}^nc_k^2$. If $C>0$, the [Markov inequality](../../../../../markov-inequality.md) gives for $\theta>0$,

$$
\mathbb P(M_n-M_0\ge x)\le\exp(-\theta x+\theta^2C/2).
$$

Minimizing at $\theta=x/C$ gives $e^{-x^2/(2C)}$. Apply the same argument to the [martingale](../../../../../martingale-split.md) $-M$ for the lower tail, and use the [union bound](../../../../../boole-s-inequality.md) to obtain the boxed result. If $C=0$, all increments vanish almost surely, so the deviation probability is zero for every $x>0$. This handles the degenerate case without dividing by zero and proves the correct bound in full.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
