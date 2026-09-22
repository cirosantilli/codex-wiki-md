<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal T_n$ be the first exit from $[1/n,1-1/n]$. On that compact interval the drift $v/2$ is bounded. The [Girsanov theorem](../../../../../../girsanov-theorem.md) therefore gives, through every fixed time $t$, a probability measure equivalent to the original one under which the stopped process $X_{\cdot\wedge\mathcal T_n}$ has Brownian increments before $\mathcal T_n$.

If $A\subset(0,1)$ has [Lebesgue measure](../../../../../../lebesgue-measure.md) zero, the [normal distribution](../../../../../../normal-distribution.md) of Brownian motion gives

$$
\mathbb P(X_t\in A,t<\mathcal T_n)=0.
$$

Since $\{t<\mathcal T\}=\bigcup_n\{t<\mathcal T_n\}$, countable subadditivity gives $\mathbb P(X_t\in A,t<\mathcal T)=0$. Thus the killed law at time $t$ is [absolutely continuous](../../../../../../absolute-continuity-of-measures.md) with respect to Lebesgue measure on $(0,1)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
