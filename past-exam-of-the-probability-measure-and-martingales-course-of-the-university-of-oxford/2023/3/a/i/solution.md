<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A discrete-time [stopping time](../../../../../stopping-time.md) for a [filtration](../../../../../filtration-probability-theory.md) $(\mathcal F_n)$ is a [random variable](../../../../../random-variable-split.md) $\tau$ taking values in $\{0,1,\ldots\}\cup\{\infty\}$ such that $\{\tau\leq n\}\in\mathcal F_n$ for every $n$. It means that whether stopping has occurred by time $n$ can be determined from the information available then.

For the first elimination time,

$$
\{\tau\leq n\}=\bigcup_{j=0}^n\{X_jY_jZ_j=0\}.
$$

Each [event](../../../../../event.md) in this finite [union](../../../../../set-union.md) belongs to $\mathcal F_j\subseteq\mathcal F_n$, by the definition of the [natural filtration](../../../../../natural-filtration.md). Therefore **$\tau$ is a stopping time**. This verification does not require first knowing whether $\tau$ is finite [almost surely](../../../../../almost-sure-convergence.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
