<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $\Delta_hf(x)=f(x+h)\overline{f(x)}$ and the unnormalized [Fourier transform](../../../../../../fourier-transform.md)

$$
\widehat g(r)=\sum_{x\in\mathbb Z_N}g(x)e(-rx/N).
$$

We state the eighth-power convention explicitly. A bounded function is $\alpha$-quadratically uniform if

$$
\boxed{\|f\|_{U^3}^8\le\alpha,\qquad
\|f\|_{U^3}^8=\mathbb E_{x,h_1,h_2,h_3}
\prod_{\epsilon\in\{0,1\}^3}\mathcal C^{|\epsilon|}f(x+\epsilon_1h_1+\epsilon_2h_2+\epsilon_3h_3),}
$$

where $\mathcal C$ means conjugation and every expectation is uniform. The expression is real and nonnegative. Applying [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) to the [multiplicative derivatives](../../../../../../multiplicative-derivative.md) gives the equivalent condition

$$
\|f\|_{U^3}^8=\frac1{N^5}\sum_{h,r}|\widehat{\Delta_h f}(r)|^4\le\alpha.
$$

This is the [Derivative identity for the Gowers U3 norm](../../../../../../derivative-identity-for-the-gowers-u3-norm.md). A set $A$ of density $\delta$ is [quadratically uniform](../../../../../../quadratic-uniformity-of-a-set.md) when its [balanced subset indicator](../../../../../../balanced-indicator-function-of-a-finite-subset.md) $1_A-\delta$ satisfies that condition, not when its unbalanced indicator does. Some definitions bound $\|f\|_{U^3}$ rather than its eighth power; that norm parameter is $\alpha^{1/8}$ in the convention here. Quadratic uniformity controls three-dimensional additive cubes and four-term progression counts; small ordinary linear Fourier coefficients alone are not the same condition.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
