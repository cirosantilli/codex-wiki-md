<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Represent a possibly randomized [statistical test](../../../../../statistical-test.md) by a function $\varphi(Y)$ taking values in $[0,1]$, its conditional probability of rejection. Its [power function](../../../../../power-function-of-a-statistical-test.md) is $\pi(\rho)=\mathbb E_\rho\varphi(Y)$, and its [size of a statistical test](../../../../../size-of-a-statistical-test.md) is the supremum of this probability over the [null hypothesis](../../../../../null-hypothesis.md). At a prescribed [significance level](../../../../../significance-level.md) $\alpha$, a [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) has at least as much power as every other level-$\alpha$ test at every parameter in the alternative.

Put $S=\sum_{j=1}^nY_j$. For any fixed alternative $0<\rho_1<\rho_0$, the [likelihood ratio](../../../../../likelihood-ratio.md) is

$$
\frac{L(\rho_1)}{L(\rho_0)}=\left(\frac{\rho_1}{\rho_0}\right)^n e^{(\rho_0-\rho_1)S},
$$

which is strictly increasing in $S$. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) therefore selects the upper tail $S>c_\alpha$. Its cutoff is determined solely by the null distribution, not by $\rho_1$, so the same [statistical test](../../../../../statistical-test.md) is most powerful against every allowed alternative and hence uniformly most powerful.

Under rate $\rho$, $S$ has a [gamma distribution](../../../../../gamma-distribution.md) with shape $n$ and rate $\rho$. For completeness, convolution starts with $\rho e^{-\rho s}$ and, if the $n$-term density is $\rho^ns^{n-1}e^{-\rho s}/(n-1)!$, convolving once more gives $\rho^{n+1}s^ne^{-\rho s}/n!$. Integrating this density by parts repeatedly gives its upper-tail probability. Consequently **reject precisely when $S>c_\alpha$**, where

$$
e^{-\rho_0c_\alpha}\sum_{j=0}^{n-1}\frac{(\rho_0c_\alpha)^j}{j!}=\alpha,
$$

and the [power function](../../../../../power-function-of-a-statistical-test.md) is

$$
\boxed{\pi(\rho)=e^{-\rho c_\alpha}\sum_{j=0}^{n-1}\frac{(\rho c_\alpha)^j}{j!}}.
$$

For $0<\alpha<1$ the continuous strictly decreasing null tail gives a unique positive cutoff, with exact size $\alpha$ and no boundary randomization.

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
