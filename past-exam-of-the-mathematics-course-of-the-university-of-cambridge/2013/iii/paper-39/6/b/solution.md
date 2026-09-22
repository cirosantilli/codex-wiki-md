<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $h_t$ and $k_t$ be predictable holdings in the stock and account, with the stochastic integrability needed for a [self-financing portfolio](../../../../../../self-financing-portfolio.md). Then $V=hS+kB$ and $dV=h\,dS+k\,dB$. The [Itô product rule](../../../../../../ito-product-rule.md) and self-financing identity give

$$
\begin{aligned}
d(ZV)&=Z\,dV+V\,dZ+d[Z,V]\\
&=\{ZhS\sigma-ZV\lambda\}\,dW
+\{ZhS\mu+ZkBr-ZVr-ZhS\sigma\lambda\}\,dt.
\end{aligned}
$$

Since $V=hS+kB$ and $\sigma\lambda=\mu-r$, the finite-variation term is zero. Therefore

$$
\boxed{d(ZV)=Z(hS\sigma-V\lambda)dW,}
$$

and the deflated wealth is a [local martingale](../../../../../../local-martingale.md).

For [zero-capital nonnegative wealth under a local deflator](../../../../../../zero-capital-nonnegative-wealth-under-a-local-deflator.md), a [nonnegative local martingale](../../../../../../nonnegative-local-martingale.md) is a [supermartingale](../../../../../../supermartingale.md), by localization and the [Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md). Under the required nonnegative-wealth condition, $ZV\ge0$ and starts at zero, so $0\le\mathbb E(Z_tV_t)\le0$. Thus $Z_tV_t=0$ almost surely at every fixed $t$. Strict positivity of $Z$ gives $V_t=0$ almost surely. Taking a countable intersection over rational times and then using continuous wealth paths strengthens this to

$$
\boxed{V_t=0\quad\text{for every }t\ge0\text{ on a single event of probability one}.}
$$

This argument only needs the local deflator, so it remains valid without promoting $ZB$ to a true [martingale](../../../../../../martingale-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
