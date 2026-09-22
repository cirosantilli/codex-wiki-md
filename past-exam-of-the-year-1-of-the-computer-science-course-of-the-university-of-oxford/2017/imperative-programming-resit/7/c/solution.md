<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use tagged [disjoint unions](../../../../../disjoint-union.md) for results that can contain either a value or an error message. This avoids ambiguity even if the item set itself contains the string `Empty queue`. The operation signatures are

$$
\boxed{\begin{aligned}
\operatorname{create}&:1\to Q,\\
\operatorname{head}&:Q\to I\sqcup M,\\
\operatorname{add}&:I\times Q\to Q,\\
\operatorname{delete}&:Q\to Q\sqcup M,\\
\operatorname{empty}&:Q\to B.
\end{aligned}}
$$

Here $1$ is a singleton, expressing that `create` takes no meaningful argument. Write successful results as $\operatorname{ok}_I(i)$ and $\operatorname{ok}_Q(q)$, and errors as $\operatorname{err}_I(e)$ and $\operatorname{err}_Q(e)$ for $e=\text{Empty queue}$. Returning an error is not returning a queue, so its result must not be silently passed to another queue operation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
