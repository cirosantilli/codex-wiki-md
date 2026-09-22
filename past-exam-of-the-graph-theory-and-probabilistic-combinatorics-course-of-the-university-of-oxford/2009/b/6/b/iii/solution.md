<h1 id="b/6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use both families of bad events in one [asymmetric Lovász local lemma](../../../../../../asymmetric-lovasz-local-lemma.md) application. Give every four-edge event parameter $x_4$ and every six-edge event parameter $x_6$. A path of length $\ell$ shares edges with at most $4\ell\Delta^3$ four-edge paths and $6\ell\Delta^5$ six-edge paths. It therefore suffices to verify

$$
k^{-2}\leq x_4(1-x_4)^{16\Delta^3}(1-x_6)^{24\Delta^5},
$$



$$
k^{-3}\leq x_6(1-x_4)^{24\Delta^3}(1-x_6)^{36\Delta^5},\qquad0<x_4,x_6<1.
$$

These slightly excessive exponents are safe even though they may count the event itself. Choose $x_4=2/k^2$ and $x_6=2/k^3$. For $k\geq C\Delta^{5/3}$, the sums of exponents times their parameters are bounded by constants times $C^{-2}\Delta^{-1/3}+C^{-3}$, uniformly in $\Delta\geq1$. Taking $C$ sufficiently large makes each product of factors at least $1/2$, for example using $(1-x)^r\geq1-rx$ and multiplying the two factors. Both displayed inequalities then hold. Positive [probability](../../../../../../probability.md) of no bad event gives **simultaneous avoidance of both lengths**. Keeping two event parameters avoids replacing the rarer six-edge events by the larger four-edge [probability](../../../../../../probability.md).

These are the [avoiding short repetitions in an edge coloring](../../../../../../avoiding-short-repetitions-in-an-edge-coloring.md) bounds, for [repetitively colored paths](../../../../../../repetitively-colored-path.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
