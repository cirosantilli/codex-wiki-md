<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

The [path lifting theorem](../../../../../path-lifting-theorem.md) says that a path $\gamma:[0,1]\to X$ has a unique lift through a covering map once its initial point in the fiber is chosen. The [homotopy lifting lemma](../../../../../homotopy-lifting-theorem-for-a-covering-map.md) says that a homotopy $H:Z\times[0,1]\to X$, with a continuous lift specified at time zero, has a unique continuous lifted homotopy. In particular a homotopy of paths with fixed endpoints preserves the endpoint of a chosen lift, since that endpoint varies continuously in a discrete fiber.

Choose $x_0\in X$ and $y_i\in p_i^{-1}(x_0)$. For $y\in Y_1$, choose a path $\gamma$ in $Y_1$ from $y_1$ to $y$, and let $F(y)$ be the endpoint of the lift of $p_1\gamma$ to $Y_2$ starting at $y_2$. Two choices of $\gamma$ are homotopic relative endpoints because $Y_1$ is simply connected. Project that homotopy and apply homotopy lifting: the lifted endpoint remains fixed. Thus $F$ is well-defined and $p_2F=p_1$.

To prove continuity without invoking covering-space classification, choose a path-connected open neighborhood $U$ of $p_1(y)$ evenly covered by both maps. Local path connectedness of $X$ permits this choice. On the sheet of $p_1^{-1}(U)$ containing $y$, append paths within that sheet to the chosen path to $y$. Path-lift uniqueness gives

$$
F=(p_2|_{V_2})^{-1}\circ p_1
$$

there, for the sheet $V_2$ containing $F(y)$. Hence $F$ is a local homeomorphism and is continuous. Construct $G:Y_2\to Y_1$ in the same way with the basepoints reversed. Lifting the very same projected paths proves $GF$ and $FG$ fix every point. Therefore

$$
\boxed{Y_1\cong Y_2\text{ by a homeomorphism commuting with the coverings}.}
$$

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
