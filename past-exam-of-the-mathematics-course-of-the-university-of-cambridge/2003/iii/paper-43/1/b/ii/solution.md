<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating the [Pareto distribution](../../../../../../../pareto-distribution.md) proposal yields $G(x)=1-(a/x)^b$ for $x\ge a$. For an independent [uniform random variable](../../../../../../../uniform-random-variable.md) $U$, solve $G(Y)=U$ to obtain the [inverse transform sampling](../../../../../../../inverse-transform-sampling.md) rule

$$
\boxed{Y=a(1-U)^{-1/b}.}
$$

Equivalently $Y=aU^{-1/b}$ because $1-U$ is also [uniformly distributed](../../../../../../../continuous-uniform-distribution.md). In implementation choose $U$ strictly between zero and one so that the inverse is finite.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
