<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take labels $y_i\in\{-1,1\}$ and fix the standard normalization in which the squared weight penalty has coefficient $1/2$. The [squared-slack support vector machine](../../../../../squared-slack-support-vector-machine.md), a form of [soft-margin support vector machine](../../../../../soft-margin-support-vector-machine.md), has [primal problem](../../../../../primal-problem.md)

$$
\boxed{\begin{aligned}
\underset{w,b,\xi}{\operatorname{minimize}}\quad&\frac12\|w\|^2+C\sum_{i=1}^m\xi_i^2,\\
\text{subject to}\quad&y_i(w\cdot x_i+b)\geq1-\xi_i,\qquad i=1,\ldots,m,\\
&\xi_i\geq0,\qquad i=1,\ldots,m.
\end{aligned}}
$$

The [slack variables of a support vector machine](../../../../../slack-variables-of-a-support-vector-machine.md) permit margin violations. Penalizing $\|w\|^2$ favors a wide [support-vector-machine margin](../../../../../support-vector-machine-margin.md), while $C>0$ sets the cost of the violations. The intercept $b$ is unpenalized, and the resulting [classifier](../../../../../classifier.md) is $h(x)=\operatorname{sign}(w\cdot x+b)$, with a fixed choice at zero. The square on $\xi_i$ is essential to the [Lagrangian dual problem](../../../../../lagrangian-dual-problem.md) below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
