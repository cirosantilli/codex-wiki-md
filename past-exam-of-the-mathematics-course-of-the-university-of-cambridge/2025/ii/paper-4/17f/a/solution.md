<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [diagonal Ramsey number](../../../../../../diagonal-ramsey-number.md) $R(t)$ is the least positive integer $n$ such that every red-blue colouring of the edges of $K_n$ contains a monochromatic $K_t$.

More generally, let $R(s,t)$ be the least $n$ forcing either a red $K_s$ or a blue $K_t$. We have

$$
R(1,t)=R(s,1)=1.
$$

Assuming the two smaller numbers exist, colour

$$
K_{R(s-1,t)+R(s,t-1)}
$$

and choose a vertex $v$. At least $R(s-1,t)$ of its incident edges are red, or at least $R(s,t-1)$ are blue. In the first case, the corresponding neighbourhood contains a red $K_{s-1}$, which extends with $v$ to a red $K_s$, or a blue $K_t$. The second case is symmetric. Thus

$$
R(s,t)\leq R(s-1,t)+R(s,t-1),
$$

which proves existence by induction.

Pascal's identity then gives the [binomial upper bound for a Ramsey number](../../../../../../binomial-upper-bound-for-a-ramsey-number.md)

$$
R(s,t)\leq\binom{s+t-2}{s-1}.
$$

Consequently, for $t\geq2$,

$$
\boxed{R(t)=R(t,t)
\leq\binom{2t-2}{t-1}
\leq2^{2t-2}<2^{2t}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
