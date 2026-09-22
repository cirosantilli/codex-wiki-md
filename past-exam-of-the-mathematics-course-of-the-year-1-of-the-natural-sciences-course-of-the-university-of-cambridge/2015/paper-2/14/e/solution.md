<h1 id="14/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**The product formula requires independent failure times.** This assumption is not stated in the original PDF. Under that intended assumption, put $s=t/T$ and use the [failure probabilities for two independent lifetimes](../../../../../failure-probabilities-for-two-independent-lifetimes.md):

$$
\boxed{P(t)=P_1(t)P_2(t)=\begin{cases}
0,&t\leq0,\\s^3,&0<t<T,\\1,&t\geq T.
\end{cases}}
$$

Its graph is a cubic increasing from $(0,0)$ to $(T,1)$, convex before reaching its plateau.

Without independence, the marginal distributions do not determine $P(t)$. The [Fréchet inequalities](../../../../../frechet-inequalities.md) give the sharp pointwise bounds

$$
\boxed{\max(0,s+s^2-1)\leq P(t)\leq s^2,\qquad0<s<1}.
$$

For example, taking $t_1=TU$ and $t_2=T\sqrt U$ with the same uniform random variable $U$ preserves both prescribed marginals but gives $P(t)=s^2$, rather than $s^3$.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [14](../../14.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
