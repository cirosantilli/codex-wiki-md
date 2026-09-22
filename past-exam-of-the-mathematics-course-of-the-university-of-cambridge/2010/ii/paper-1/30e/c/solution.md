<h1 id="30e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $[u]=u_r-u_l$ and $[f]=u_r^2/2-u_l^2/2$. Splitting the test-function integral along $x=s(t)$ and integrating by parts gives a remaining interface contribution

$$
\int\bigl(s'(t)[u]-[f]\bigr)\phi(s(t),t)\,dt.
$$

For example the normal to the interface in $(x,t)$ coordinates is proportional to $(1,-s')$, so the jump in the conserved spacetime flux $(u^2/2,u)$ has normal component $[f]-s'[u]$. Since the traces of the [test function](../../../../../../test-function.md) are arbitrary, the interior weak equation holds if and only if $s'[u]=[f]$. At a genuine jump $[u]\ne0$, this is

$$
\boxed{s'(t)=\frac{u_l(t)+u_r(t)}2.}
$$

This is the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md). An initial-value weak formulation also requires the prescribed initial [trace](../../../../../../matrix-trace.md); the jump condition alone concerns the interior equation. The source's reference to “(1)” is to the displayed Burgers equation, not a different PDE.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30E](../../30e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
