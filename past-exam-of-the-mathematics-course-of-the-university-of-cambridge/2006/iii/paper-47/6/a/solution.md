<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First distinguish a complete-data calculation, conditional on the missing counts, from optimization of the observed-data likelihood. Introduce death counts $D_j=\sum_{i=1}^jn_{ij}$, survivor counts $S_j=A_{1j}$, observed recapture counts $C_j=\sum_{i=1}^{j-1}m_{ij}$ and unobserved-alive counts $U_j=A_{2j}$. Terms involving these probabilities in the complete-data log likelihood are

$$
\ell=\sum_{j=1}^{J-1}[D_j\log(1-\phi_j)+S_j\log\phi_j]
+\sum_{j=2}^J[C_j\log P_j+U_j\log(1-P_j)]+\text{constant}.
$$

The survival score is $S_j/\phi_j-D_j/(1-\phi_j)$ and the detection score is $C_j/P_j-U_j/(1-P_j)$. Their derivatives are nonpositive, and strictly negative whenever their respective total counts are positive. The interior roots, with boundary interpretations if a success or failure count vanishes, are therefore

$$
\boxed{\widehat\phi_j=\frac{S_j}{S_j+D_j},\qquad
\widehat P_j=\frac{C_j}{C_j+U_j}.}
$$

Substituting the survivor and unobserved-alive totals gives

$$
\widehat\phi_j=
\frac{\sum_{i=1}^j\sum_{s=j+1}^J(m_{is}+n_{is})}
{\sum_{i=1}^j(\sum_{s=j+1}^Jm_{is}+\sum_{s=j}^Jn_{is})},
\quad
\widehat P_j=
\frac{\sum_{i=1}^{j-1}m_{ij}}
{\sum_{i=1}^{j-1}\sum_{s=j}^J(m_{is}+n_{is})}.
$$

These are the requested complete-data maximizing ratios. Here $n_{iJ}$ denotes the terminal missing count discussed in part (b); pre-release cells and nonexistent release cohorts contribute zero. If a denominator is zero, the likelihood is constant in that parameter rather than defining a $0/0$ estimate. Also $P_1$ does not occur in this likelihood and has no identified maximum. With unobserved $n$, these ratios alone do not yet supply an observed-data estimate; the [EM algorithm](../../../../../../expectation-maximization-algorithm.md) below supplies the missing-count expectations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
