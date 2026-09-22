<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The two descendant branches of an equal-rate [Jukes-Cantor model](../../../../../jukes-cantor-model.md) compose to a single branch of duration $2T$. More explicitly, the model is symmetric, so summing over the ancestral base gives $\sum_a\pi_aP_{ai}(T)P_{aj}(T)$ and a total mismatch probability $\tfrac34(1-e^{-2\mu T})$. Thus use the pairwise difference fraction directly with $t=2T$, rather than halving the differences and correcting the halves separately:

$$
\begin{aligned}
\widehat\mu
&=-\frac{\ln(1-4\times0.29/3)}{29\times10^6}\\
&=\boxed{1.68568\times10^{-8}\ \text{year}^{-1}}.
\end{aligned}
$$

This is the parameter in the printed formula of (c). For a [mutation rate](../../../../../mutation-rate.md) measured as actual changes per site per year, the conversion derived in (b) gives

$$
\boxed{\widehat r=\frac34\widehat\mu=1.26426\times10^{-8}\ \text{site}^{-1}\text{year}^{-1}}.
$$

The latter is directly comparable to the naive estimate in (a): allowing repeated changes raises that estimate by about $26.4\%$. The exponent parameter and actual event rate are two conventions for the same fitted process, not two different biological estimates.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
