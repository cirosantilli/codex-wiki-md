<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose for contradiction that some $q\in\mathcal P_n$ satisfies

$$
\|f-q\|_\infty\lt a_*:=\min_i a_i.
$$

At $t_i$,

$$
p(t_i)-q(t_i)=[f(t_i)-q(t_i)]-(-1)^ia_i.
$$

Because $|f(t_i)-q(t_i)|\lt a_i$, the values $p(t_i)-q(t_i)$ have strictly alternating signs. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) therefore gives at least one root of $p-q$ in each of the $n+1$ intervals $(t_i,t_{i+1})$. A nonzero polynomial of degree at most $n$ cannot have $n+1$ distinct roots. If $p-q$ were identically zero, its error at $t_i$ would be $a_i\geq a_*$, also a contradiction. Hence

$$
\boxed{E_n(f)\geq\min_{1\leq i\leq n+2}a_i}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
