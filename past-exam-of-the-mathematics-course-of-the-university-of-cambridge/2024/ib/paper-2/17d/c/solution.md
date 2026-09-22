<h1 id="17d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

From the same value $y_n$, the two trial steps are

$$
y_F=(I+hM)y_n,
\qquad
 y_B=(I-hM)^{-1}y_n.
$$

The exact step and the two approximations expand as

$$
\begin{aligned}
e^{hM}y_n&=\left(I+hM+\frac12h^2M^2+O(h^3)\right)y_n,\\
y_F&=(I+hM)y_n,\\
y_B&=\left(I+hM+h^2M^2+O(h^3)\right)y_n.
\end{aligned}
$$

Thus their leading local errors have opposite signs, and the [Milne device for forward and backward Euler](../../../../../../milne-device-for-forward-and-backward-euler.md) estimates either magnitude by

$$
\boxed{E_n=\frac12\lVert y_B-y_F\rVert
=\frac12h^2\lVert M^2y_n\rVert+O(h^3)}.
$$

Use backward Euler as the accepted step because it is A-stable. Reject a trial if $E_n$ exceeds the prescribed local tolerance; otherwise accept $y_B$ and choose, with a safety factor $s<1$,

$$
\boxed{h_{\rm new}=s h
\left(\frac{\mathrm{tol}}{E_n}\right)^{1/2}}.
$$

The small steps resolve the initial fast transient. Once its amplitude has decayed, the error estimator permits much larger steps, while the accepted backward-Euler evolution remains stable. This controls the error without paying the forward-Euler stability restriction throughout the integration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17D](../../17d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
