<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Until the walk first reaches $B$, it is the [simple random walk](../../../../../../simple-random-walk.md) on a path of length $n$ with reflection at the endpoint $A$. If $h_i$ is the [expected hitting time](../../../../../../expected-hitting-time.md) of $B$ from the vertex at distance $i$ from $A$, then

$$
h_n=0,
\qquad h_0=1+h_1,
\qquad h_i=1+\frac12(h_{i-1}+h_{i+1})\quad(1\leq i<n).
$$

Solving this second-difference equation gives $h_i=n^2-i^2$. Therefore

$$
\boxed{\mathbb E_A[T_B]=n^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
