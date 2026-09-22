<h1 id="27h/solution">Solution</h1>

↑ **Parent:** [27H](../27h.md)

For a nonnegative measurable $f$, define

$$
f_n(x)=2^{-n}\left\lfloor2^n\min(f(x),n)\right\rfloor.
$$

Each $f_n$ takes only finitely many values, its level sets are measurable, and $f_n(x)\to f(x)$ pointwise. Thus measurable nonnegative functions are pointwise limits of [simple functions](../../../../../approximation-by-nonnegative-simple-functions.md).

If $f$ is integrable, the same functions satisfy $0\leq f_n\leq f$ and converge pointwise. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives

$$
\int_E|f_n-f|\,d\mu\longrightarrow0.
$$

They are integrable because they are bounded above by $f$.

If $0\leq f\leq M$, instead set

$$
g_n=2^{-n}\lfloor2^nf\rfloor.
$$

This has finitely many values and

$$
0\leq f-g_n<2^{-n}
$$

everywhere, so $g_n\to f$ uniformly.

## ↑ Ancestors (10)

1. [27H](../27h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
