<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $\mathbb EX=0$, the [moment-generating function](../../../../../../moment-generating-function.md) series and the [Bernstein moment condition](../../../../../../bernstein-moment-condition.md) imply, for $|\lambda|b<1$,

$$
\begin{aligned}
\mathbb Ee^{\lambda X}
&=1+\sum_{k=2}^{\infty}\frac{\lambda^k\mathbb E[X^k]}{k!}\\
&\leq1+\frac{\nu\lambda^2}{2}
\sum_{k=2}^{\infty}(|\lambda|b)^{k-2}\\
&=1+\frac{\nu\lambda^2}{2(1-|\lambda|b)}\\
&\leq\exp\left(\frac{\nu\lambda^2}{2(1-|\lambda|b)}\right).
\end{aligned}
$$

For $|\lambda|<1/(2b)$, the denominator satisfies $1-|\lambda|b>1/2$, so

$$
\mathbb Ee^{\lambda X}\leq e^{\nu\lambda^2}
=e^{\lambda^2(2\nu)/2}.
$$

**Thus $X$ is sub-exponential with parameters $(2\nu,2b)$.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
