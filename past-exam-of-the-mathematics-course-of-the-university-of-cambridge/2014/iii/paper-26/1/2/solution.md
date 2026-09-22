<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $0<x<r$, the exit time is at least one. Since $\{\eta\geq n\}=\{\eta>n-1\}\in\mathcal F_{n-1}$, this event is independent of $X_n$. The [Tonelli theorem](../../../../../../tonelli-theorem.md) gives

$$
\mathbb E|X_\eta|
=\sum_{n\geq1}\mathbb E\bigl[|X_n|\mathbf1_{\{\eta=n\}}\bigr]
\leq\sum_{n\geq1}\mathbb E\bigl[|X_n|\mathbf1_{\{\eta\geq n\}}\bigr]
=\mathbb E|X_1|\sum_{n\geq1}\mathbb P(\eta\geq n).
$$

Therefore the [integrability of a stopped random-walk increment](../../../../../../integrability-of-a-stopped-random-walk-increment.md) bound is

$$
\boxed{\mathbb E|X_\eta|\leq\mathbb E|X_1|\,\mathbb E\eta<\infty.}
$$

It is the survival event, not the exit-at-$n$ event, that is independent of the next increment. The selected exit increment need not have the same distribution or mean as $X_1$.

For $r\leq x$, the printed variable $X_\eta=X_0$ is undefined because the increment sequence starts at one. Either restrict this part to $0<x<r$, or make the harmless additional convention $X_0=0$. With that convention the conclusion also holds in the immediate-exit case. **The integrability assertion needs this indexing qualification.**

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
