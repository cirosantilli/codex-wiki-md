<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For these increasing warps, the [square-root velocity function](../../../../../../../square-root-velocity-function.md) is $Q(h)(t)=\sqrt{h'(t)}$. The [chain rule](../../../../../../../chain-rule.md) gives

$$
Q(h_i\circ\gamma)(t)
=Q(h_i)(\gamma(t))\sqrt{\gamma'(t)}.
$$

Therefore

$$
\begin{aligned}
\lVert Q(h_i\circ\gamma)-Q(h_j\circ\gamma)\rVert_2^2
&=\int_0^1
|Q(h_i)(\gamma(t))-Q(h_j)(\gamma(t))|^2\gamma'(t)\,dt\\
&=\int_0^1|Q(h_i)(u)-Q(h_j)(u)|^2\,du,
\end{aligned}
$$

where the last equality again uses the [change of variables formula](../../../../../../../change-of-variables-formula.md). Taking square roots proves invariance under common right composition by $\gamma$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 225](../../../../paper-225-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
