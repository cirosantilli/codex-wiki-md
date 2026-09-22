<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $g:\mathbb R\to\mathbb R$ be continuously differentiable. Applying the Poincaré inequality for $p$ to $g\circ\phi$ and using the [chain rule](../../../../../../chain-rule.md) gives

$$
\begin{aligned}
\operatorname{Var}_q(g(Y))
&=\operatorname{Var}_p(g(\phi(X)))\\
&\leq c^2\mathbb E_p\lVert g'(\phi(X))\nabla\phi(X)\rVert^2\\
&\leq c^2L^2\mathbb E_q[g'(Y)^2].
\end{aligned}
$$

**Thus the [Pushforward of a Poincaré inequality by a Lipschitz function](../../../../../../pushforward-of-a-poincare-inequality-by-a-lipschitz-function.md) gives a $cL$-Poincaré inequality for $q$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
