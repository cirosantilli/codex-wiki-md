<h1 id="5/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let

$$
a=e^{\beta z_{n-1}},\qquad b=e^{\beta z_n},\qquad c=e^{\beta z_{n-2}},
$$

and let $C$ be the common [partial likelihood](../../../../../../../partial-likelihood.md) contribution from the first $n-3$ observations. Since $t_{n-2}>x_{n-2}$, the three possible complete-data tail orderings and their partial likelihoods are

$$
\begin{array}{c|c}
t_{n-2}<x_{n-1}<x_n&C\dfrac{c}{a+b+c}\dfrac{a}{a+b}\\[6pt]
x_{n-1}<t_{n-2}<x_n&C\dfrac{a}{a+b+c}\dfrac{c}{b+c}\\[6pt]
x_{n-1}<x_n<t_{n-2}&C\dfrac{a}{a+b+c}\dfrac{b}{b+c}.
\end{array}
$$

Their sum is

$$
C\left[
\frac{c}{a+b+c}\frac{a}{a+b}
+\frac{a}{a+b+c}\frac{c+b}{b+c}
\right]
=C\frac{a}{a+b}.
$$

When individual $n-2$ is [right-censored](../../../../../../../right-censoring.md) at $x_{n-2}$, that individual leaves the [risk set](../../../../../../../risk-set.md) before the event at $x_{n-1}$, so the directly calculated [Cox partial likelihood](../../../../../../../cox-partial-likelihood.md) is also $C,a/(a+b)$. Summing over the unobserved compatible event orderings therefore reproduces the censored-data partial likelihood.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
