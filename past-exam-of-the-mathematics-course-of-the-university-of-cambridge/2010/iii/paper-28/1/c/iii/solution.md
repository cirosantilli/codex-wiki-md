<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\rho=p/q\in(0,1)$ and $M=\sup_{n\geq0}S_n$. For $k\geq1$, $\{M\geq k\}=\{H_k<\infty\}$, so part (ii) gives $\mathbb P(M\geq k)=\rho^k$. Since $\mathbb P(M\geq0)=1$, taking differences gives

$$
\boxed{\mathbb P(M=j)=\rho^j-\rho^{j+1}=(1-\rho)\rho^j,\qquad j=0,1,\ldots.}
$$

This is the [geometric distribution](../../../../../../../geometric-distribution.md) of parameter $1-p/q$ on the failures-before-first-success convention, with support $\{0,1,\ldots\}$. Its [expected value](../../../../../../../expected-value.md) is $\rho/(1-\rho)=p/(q-p)$, so the bound in part (b)(ii) is attained. This proves the [maximum of a downward-biased random walk](../../../../../../../maximum-of-a-downward-biased-random-walk.md) formula.

The time-zero convention is necessary here. If $M_1=\sup_{n\geq1}S_n$, then the first step can be $-1$ and the walk may never return to zero. Using the same [hitting probability](../../../../../../../hitting-probability.md) calculation after that step gives $\mathbb P(M_1=-1)=q(1-\rho)=q-p>0$. Also $\mathbb P(M_1\geq0)=p+q\rho=2p$, while its tails at positive $k$ remain $\rho^k$. Its masses are therefore

$$
\mathbb P(M_1=-1)=q-p,\qquad
\mathbb P(M_1=0)=2p-\rho,\qquad
\mathbb P(M_1=j)=(1-\rho)\rho^j\quad(j\geq1).
$$

Thus the printed geometric conclusion is correct for the standard maximum that includes $S_0=0$, and false for a supremum restricted to the positive times.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
