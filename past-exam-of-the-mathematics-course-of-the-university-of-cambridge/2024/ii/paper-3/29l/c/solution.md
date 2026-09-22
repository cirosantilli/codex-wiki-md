<h1 id="29l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a node with time $n-1$ price $s$, choose the stock holding

$$
\Delta_n(s)=\frac{V(n,s(1+b))-V(n,s(1+a))}{s(b-a)}.
$$

The two possible values of the stock position differ by exactly the difference between the two continuation claims. Choose the bank holding so that total wealth is $V(n-1,s)$. The pricing recursion makes its next value equal to the appropriate continuation value in both states. Backward induction from $V(N,s)=g(s)$ therefore replicates $g(S_N)$ from initial capital $V(0,S_0)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29L](../../29l.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
