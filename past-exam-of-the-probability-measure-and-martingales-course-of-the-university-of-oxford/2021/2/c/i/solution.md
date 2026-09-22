<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The conditions on the [cumulative distribution function](../../../../../cumulative-distribution-function.md) imply $0<X_n\leq2$ [almost surely](../../../../../almost-sure-convergence.md). With $\mathcal H_n=\sigma(X_1,\ldots,X_n)$, adjoin $Y_0=1$ and the trivial $\mathcal H_0$. The [random variables](../../../../../random-variable-split.md) $Y_n$ are nonnegative, [adapted](../../../../../adapted-process.md), and bounded by $2^n$ at each fixed time. [Independence](../../../../../independent-random-variables.md) and $\mathbb EX_{n+1}=1$ give

$$
\mathbb E[Y_{n+1}\mid\mathcal H_n]=Y_n\mathbb EX_{n+1}=Y_n.
$$

Thus this is the [product martingale from independent mean-one factors](../../../../../product-martingale-from-independent-mean-one-factors.md), with $\mathbb EY_n=1$. The [almost sure supermartingale convergence theorem](../../../../../almost-sure-supermartingale-convergence-theorem.md) states that a nonnegative [supermartingale](../../../../../supermartingale.md) converges [almost surely](../../../../../almost-sure-convergence.md) to a finite [integrable random variable](../../../../../integrable-random-variable.md). Applied to this nonnegative [martingale](../../../../../martingale-split.md), it shows $Y_n\to Y_\infty<\infty$ [almost surely](../../../../../almost-sure-convergence.md). Every convergent real [sequence](../../../../../sequence.md) is bounded, so **$\sup_{n\geq1}Y_n<\infty$ almost surely**.

The printed maximum can in fact be taken literally here. If $X_1=1$ [almost surely](../../../../../almost-sure-convergence.md), all products equal $1$. Otherwise the [strict Jensen equality criterion](../../../../../strict-jensen-equality-criterion.md), applied to the [strictly convex function](../../../../../strictly-convex-function.md) $t\mapsto-\sqrt t$ on $(0,\infty)$, gives $q=\mathbb E\sqrt{X_1}<1$. [Independence](../../../../../independent-random-variables.md) yields $\mathbb E\sqrt{Y_n}=q^n$. By [Markov's inequality](../../../../../markov-s-inequality.md), $\sum_n\mathbb P(Y_n>\varepsilon)\leq\varepsilon^{-1/2}\sum_nq^n<\infty$ for every $\varepsilon>0$. The [First Borel-Cantelli lemma](../../../../../borel-cantelli-first-lemma.md) and the countable choices $\varepsilon=1/m$ give $Y_n\to0$ [almost surely](../../../../../almost-sure-convergence.md). Since $Y_1>0$, a [sequence](../../../../../sequence.md) with this limit attains its positive supremum among finitely many initial terms. This is an instance of [fractional moment decay of independent mean-one products](../../../../../fractional-moment-decay-of-independent-mean-one-products.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
