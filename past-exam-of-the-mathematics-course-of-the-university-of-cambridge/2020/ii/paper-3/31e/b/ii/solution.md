<h1 id="31e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For

$$
V(x,y)=\frac{x^2}{2}+g(y),
$$

the [orbital derivative](../../../../../../../orbital-derivative.md) is

$$
\dot V=x(-2x+x^3+\sin2y)+g'(y)(-x-y^3).
$$

Choosing $g'(y)=\sin2y$ cancels the mixed term. Taking $g(0)=0$ gives

$$
g(y)=\int_0^y\sin(2s)\,ds
=\frac{1-\cos2y}{2}=\sin^2y,
$$

so

$$
\boxed{V(x,y)=\frac{x^2}{2}+\sin^2y}.
$$

This function has [positive definiteness](../../../../../../../positive-definiteness-of-a-lyapunov-function.md) near the origin, and

$$
\dot V
=-2x^2+x^4-y^3\sin2y
=-x^2(2-x^2)-y^3\sin2y.
$$

For $|x|<1$ and $|y|<1$, both terms are nonpositive and equality holds only at $(0,0)$. Thus $V$ is a [strict Lyapunov function](../../../../../../../strict-lyapunov-function.md) near the origin, and the [Second Lyapunov theorem](../../../../../../../second-lyapunov-theorem.md) proves that the origin is asymptotically stable.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [31E](../../../31e.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
