<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $S(t)=\mathbb P(T>t)$ for the [survival function](../../../../../../survival-function.md); this is the function denoted $F_T$ in the survival notation. For a proper continuous event-time distribution with [hazard function](../../../../../../hazard-function.md) $h$, its [cumulative hazard function](../../../../../../cumulative-hazard-function.md) is $H(t)=\int_0^th(s)ds=-\log S(t)$. The [probability integral transform](../../../../../../probability-integral-transform.md) makes $S(T)$ uniform on $(0,1)$, including when $S$ has flat intervals: those intervals have zero event [probability](../../../../../../probability.md). Consequently

$$
\mathbb P(H(T)>u)=\mathbb P(S(T)<e^{-u})=e^{-u},\qquad u\geq0.
$$

Thus the [cumulative hazard probability transformation](../../../../../../cumulative-hazard-probability-transformation.md) gives $\boxed{H(T)\sim\operatorname{Exponential}(1)}$. No strict monotonicity of $H$ is needed on intervals that carry no event mass. The usual proper continuous survival law is essential; an atom of subjects who never fail would instead require separate treatment of the mass at infinity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
