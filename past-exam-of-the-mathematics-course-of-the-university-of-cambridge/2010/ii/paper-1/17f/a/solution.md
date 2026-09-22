<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The diagonal [diagonal Ramsey number](../../../../../../diagonal-ramsey-number.md) $R(s)$ is the least $n$ such that every red-blue edge coloring of $K_n$ contains a monochromatic $K_s$. More generally let $R(s,t)$ require a red $K_s$ or blue $K_t$. The base cases are $R(1,t)=R(s,1)=1$. Given $R(s-1,t)+R(s,t-1)$ vertices, select one vertex. Either it has at least $R(s-1,t)$ red neighbors or at least $R(s,t-1)$ blue neighbors. Applying the corresponding smaller problem and, when needed, adjoining that selected vertex gives

$$
R(s,t)\leq R(s-1,t)+R(s,t-1).
$$

Induction and Pascal's identity now prove existence and

$$
\boxed{R(s)=R(s,s)\leq\binom{2s-2}{s-1}\leq2^{2s-2}<4^s.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
