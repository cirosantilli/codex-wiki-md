<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $e(A)$ count internal edges of the [hypercube graph](../../../../../../hypercube-graph.md). Since each vertex has degree $n$, its [edge boundary](../../../../../../edge-boundary-in-a-graph.md) is $b_e(A)=n|A|-2e(A)$. The [edge-isoperimetric inequality in the discrete cube](../../../../../../edge-isoperimetric-inequality-in-the-discrete-cube.md) gives $e(A)\le |A|\log_2|A|/2$, hence $b_e(A)\ge |A|(n-\log_2|A|)$.

For completeness, the [entropy proof of cube edge-isoperimetry](../../../../../../entropy-proof-of-cube-edge-isoperimetry.md) splits the final coordinate into sections of sizes $a,b$. Their internal edges contribute at most $(a\log_2a+b\log_2b)/2$ by induction, and their crossing edges at most $\min(a,b)$. For $m=a+b$ and $t=\min(a,b)/m$, the [binary entropy function](../../../../../../binary-entropy-function.md) satisfies $H_2(t)\ge2t$, so $a\log_2a+b\log_2b+2\min(a,b)\le m\log_2m$. The convention is $0\log_20=0$.

A $k$-dimensional coordinate subcube has $2^k$ vertices and $k2^{k-1}$ internal edges, attaining the bound. Therefore

$$
\boxed{f(2^k)=2^k(n-k)}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
