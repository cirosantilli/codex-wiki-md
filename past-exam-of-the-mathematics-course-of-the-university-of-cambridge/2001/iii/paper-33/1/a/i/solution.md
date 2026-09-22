<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $C=\int_{\mathbb R}f(x)\,dx$, so $0<C<\infty$. The finite envelope condition means that $f\leq Mg$ almost everywhere; in particular, the proposal must cover the support of the target.

For each [independent](../../../../../../../independent-random-variables.md) proposal $Y\sim g$, generate an [independent](../../../../../../../independent-random-variables.md) $U\sim\operatorname{Unif}(0,1)$ and accept $Y$ precisely when

$$
\boxed{U\leq\frac{f(Y)}{Mg(Y)}.}
$$

Discard a rejected proposal and continue. The ratio is in $[0,1]$ and is needed only where $g(Y)>0$. Neither evaluation of $C$ nor prior knowledge of the normalized target is required.

To prove the output law, for any measurable set $D$ the joint [probability](../../../../../../../probability.md) of acceptance and a proposal in $D$ is

$$
\mathbb P(Y\in D,\mathrm{accept})
=\int_Dg(y)\frac{f(y)}{Mg(y)}\,dy
=\frac1M\int_Df(y)\,dy.
$$

Dividing by the total acceptance [probability](../../../../../../../probability.md) $C/M$ gives $\int_D f(y)/C\,dy$, the target [probability](../../../../../../../probability.md). [Independent](../../../../../../../independent-random-variables.md) proposal-uniform pairs give [independent](../../../../../../../independent-random-variables.md) accepted observations. With a finite proposal list there can be no accepted value; with continued [independent](../../../../../../../independent-random-variables.md) trials, acceptance eventually occurs almost surely because $C/M>0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
