<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $\alpha>0$, integration and [independence of random variables](../../../../../independent-random-variables.md) give

$$
\mathbb EU_1^\alpha=\frac1b\int_0^bu^\alpha\,du=\frac{b^\alpha}{1+\alpha},\qquad \mathbb EW_n^\alpha=\left(\frac{b^\alpha}{1+\alpha}\right)^n.
$$

By the [fractional moment criterion for convergence in probability](../../../../../fractional-moment-criterion-for-convergence-in-probability.md),

$$
\mathbb P(W_n>\varepsilon)\leq\varepsilon^{-\alpha}\left(\frac{b^\alpha}{1+\alpha}\right)^n.
$$

The parenthesized factor is less than one precisely when $\alpha\log b-\log(1+\alpha)<0$. This expression vanishes at $\alpha=0$ and has [derivative](../../../../../derivative.md) $\log b-1$ there. If $b<e$, the [derivative](../../../../../derivative.md) is negative, so some sufficiently small $\alpha>0$ makes the factor strictly less than one. The bound then tends to zero geometrically, proving

$$
\boxed{W_n\longrightarrow0\quad\text{in probability for every }0<b<e.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
