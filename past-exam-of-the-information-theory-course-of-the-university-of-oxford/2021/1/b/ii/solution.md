<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Index correction:** the printed definition only permits $i\leq n$, although the required average includes $i=n+1$. Extend the same deletion formula to $1\leq i\leq n+1$. Without that extension the final summand is undefined; there is no new sample or different estimator to supply.

For a fixed outcome of the sample and a fixed symbol $x$, put $A_j=\mathbf1_{\{X_j=x\}}$. The leave-one-out [empirical distribution](../../../../../type-information-theory.md) then satisfies

$$
\begin{aligned}
\sum_{i=1}^{n+1}\widehat q_{n,i}(x)
&=\frac1n\sum_{i=1}^{n+1}\left(\sum_{j=1}^{n+1}A_j-A_i\right)\\
&=\frac1n\left((n+1)\sum_{j=1}^{n+1}A_j-\sum_{i=1}^{n+1}A_i\right)
=\sum_{j=1}^{n+1}A_j.
\end{aligned}
$$

Dividing by $n+1$ gives **$\widehat p_{n+1}=(n+1)^{-1}\sum_{i=1}^{n+1}\widehat q_{n,i}$.** Each of the $n+1$ [indicator functions](../../../../../indicator-function.md) was counted exactly $n$ times before division by $n$. This [leave-one-out identity for empirical distributions](../../../../../leave-one-out-identity-for-empirical-distributions.md) is deterministic; [independence](../../../../../independent-random-variables.md) plays no part in this part.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
