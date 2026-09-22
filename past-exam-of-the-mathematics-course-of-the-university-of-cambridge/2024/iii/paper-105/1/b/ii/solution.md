<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $u(x)=\sin|x|$, the ordinary derivative away from zero is

$$
g(x)=
\begin{cases}
-\cos x,&-\pi<x<0,\\
\cos x,&0<x<\pi.
\end{cases}
$$

This bounded function is locally integrable. For a [test function](../../../../../../../test-function.md) $\varphi$, [integration by parts](../../../../../../../integration-by-parts.md) on $(-\pi,0)$ and $(0,\pi)$ produces boundary terms at zero which cancel because $u$ is continuous there and $u(0)=0$. Hence

$$
\int_{-\pi}^{\pi}u\varphi'=-\int_{-\pi}^{\pi}g\varphi.
$$

Therefore $u$ has the [weak derivative](../../../../../../../weak-derivative.md)

$$
\boxed{u'(x)=\operatorname{sgn}(x)\cos|x|\quad\text{for almost every }x.}
$$

The jump in the ordinary derivative creates no [Dirac delta function](../../../../../../../dirac-delta-function.md); such a term would arise from a jump in the function itself.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
