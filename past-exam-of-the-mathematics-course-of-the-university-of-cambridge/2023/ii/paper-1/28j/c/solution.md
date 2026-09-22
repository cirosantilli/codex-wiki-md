<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Condition on $N_t=n$. By [Poisson process conditional arrival times](../../../../../../poisson-process-conditional-arrival-times.md), the jump times are the ordered version of independent $U_1,\ldots,U_n$ uniformly distributed on $[0,t]$. The sum is symmetric in the marked pairs, and the marks are independent, so

$$
\begin{aligned}
&\mathbb E\left[
\left.
\exp\left\{\theta\sum_{i=1}^{N_t}g(J_i,X_i)\right\}
\right|N_t=n\right]\\
&\qquad=
\left[
\frac1t\int_0^t
\mathbb E\left(e^{\theta g(s,X_1)}\right)ds
\right]^n.
\end{aligned}
$$

Write the bracket as $a$. Averaging over the [Poisson distribution](../../../../../../poisson-distribution.md) of $N_t$ gives

$$
\begin{aligned}
\mathbb E\exp\left\{\theta\sum_{i=1}^{N_t}g(J_i,X_i)\right\}
&=e^{-\lambda t}\sum_{n=0}^\infty
\frac{(\lambda t a)^n}{n!}\\
&=\exp\{\lambda t(a-1)\}\\
&=\exp\left\{
\lambda\int_0^t
\left(\mathbb E(e^{\theta g(s,X_1)})-1\right)ds
\right\}.
\end{aligned}
$$

This is the [exponential formula for a marked Poisson sum](../../../../../../exponential-formula-for-a-marked-poisson-sum.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
