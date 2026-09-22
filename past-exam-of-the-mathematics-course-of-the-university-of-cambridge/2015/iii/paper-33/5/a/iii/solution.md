<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Continuity of the [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) gives the [probability integral transform](../../../../../../../probability-integral-transform.md): $F(T)$ is uniform on $(0,1)$. Hence $S(T)=1-F(T)$ is also uniform, and the [cumulative hazard probability transformation](../../../../../../../cumulative-hazard-probability-transformation.md) gives

$$
H(T)=-\log S(T),\qquad
\mathbb P\{H(T)>x\}=\mathbb P\{S(T)<e^{-x}\}=e^{-x},\quad x\geq0.
$$

Thus

$$
\boxed{H(T)\sim\operatorname{Exp}(1).}
$$

The [exponential distribution](../../../../../../../exponential-distribution.md) has rate and mean one here. This proof does not require a strictly increasing cumulative hazard: intervals with zero density carry no probability mass. It assumes a proper continuous finite survival time, without an atom at infinity.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
