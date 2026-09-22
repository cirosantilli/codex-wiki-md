<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove the [Convex Poincaré inequality](../../../../../../convex-poincare-inequality.md). For a differentiable convex function $h:[0,1]\to\mathbb R$ and independent copies $U,U'$ supported on $[0,1]$, convexity gives

$$
(h(U)-h(U'))^2
\leq h'(U)^2\mathbf1_{\{U>U'\}}
+h'(U')^2\mathbf1_{\{U'<U\}}.
$$

Taking expectations and using $\operatorname{Var}(h(U))=\frac12\mathbb E(h(U)-h(U'))^2$ gives

$$
\operatorname{Var}(h(U))\leq\mathbb Eh'(U)^2.
$$

Applying this conditional inequality coordinate by coordinate in the [Efron–Stein inequality](../../../../../../efron-stein-inequality.md) proves

$$
\operatorname{Var}(f(X))\leq
\mathbb E\sum_i(\partial_if(X))^2
=\mathbb E\lVert\nabla f(X)\rVert^2\leq1.
$$

Since $-g$ is convex and has the same gradient norm as $g$, the same argument gives $\operatorname{Var}(g(X))\leq1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
