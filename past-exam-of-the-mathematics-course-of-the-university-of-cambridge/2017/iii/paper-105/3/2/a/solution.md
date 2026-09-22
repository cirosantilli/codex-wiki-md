<h1 id="3/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A bounded [weak solution](../../../../../../../weak-solution.md) satisfies

$$
\boxed{\int_0^\infty\!\int_{\mathbb R}\bigl(u\varphi_t+f(u)\varphi_x\bigr)dx\,dt+\int_{\mathbb R}u_0(x)\varphi(0,x)dx=0}
$$

for every compactly supported $C^1$ [test function](../../../../../../../test-function.md), of either sign, allowed to meet $t=0$. Across a moving jump $x=s(t)$ with distinct left/right constant states, the distributional delta coefficient vanishes exactly when the [Rankine-Hugoniot condition](../../../../../../../rankine-hugoniot-conditions.md) holds:

$$
\boxed{s'(t)(u_R-u_L)=f(u_R)-f(u_L).}
$$

It is required on every interface of a piecewise constant solution; the initial trace must also agree with the data.

For nonuniqueness respecting the paper's global bound on $f'$, use the [bounded-derivative Burgers flux](../../../../../../../bounded-derivative-burgers-flux.md) $f(z)=z^2/2$ on $|z|\le1$ and $f(z)=|z|-1/2$ outside. It is $C^1$ and $|f'|\le1$. Take data $-1$ for $x<0$, $1$ for $x>0$. A stationary jump obeys the condition because $f(-1)=f(1)$. Another weak solution is the [rarefaction wave](../../../../../../../rarefaction-wave.md)

$$
u(t,x)=\begin{cases}-1,&x\le-t,\\x/t,&-t<x<t,\\1,&x\ge t.\end{cases}
$$

The fan solves the equation inside each smooth region, is continuous at its edges, and has the same local $L^1$ initial trace. Thus **weak solutions are not unique**. The stationary expansion shock violates the entropy inequality, whereas the fan is admissible; using the unmodified quadratic flux alone would miss the printed global bounded-derivative hypothesis.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
