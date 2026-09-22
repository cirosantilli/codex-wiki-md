<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [extended real numbers](../../../../../../extended-real-number-line.md) $\overline{\mathbb R}=\mathbb R\cup\{-\infty,+\infty\}$. A [proper convex function](../../../../../../proper-convex-function.md) never takes $-\infty$ and is finite somewhere. Its [effective domain](../../../../../../effective-domain.md) is

$$
\boxed{\operatorname{dom}f=\{x\in\mathbb R^n:f(x)<+\infty\}}.
$$

For a [proper extended-real function](../../../../../../proper-extended-real-function.md), [convexity](../../../../../../convex-function.md) means

$$
f((1-t)x+ty)\leq(1-t)f(x)+tf(y),\qquad x,y\in\mathbb R^n,\quad0<t<1.
$$

The endpoint cases are identities; taking $0<t<1$ avoids the ambiguous product $0\cdot(+\infty)$. Equivalently, its [epigraph](../../../../../../epigraph.md) is a [convex set](../../../../../../convex-set.md). In particular, the [effective domain](../../../../../../effective-domain.md) is a [convex set](../../../../../../convex-set.md). Properness is an additional condition: it rules out the identically $+\infty$ function and all $-\infty$ values, rather than requiring finiteness everywhere.

For $x\in\operatorname{dom}f$, the [subdifferential](../../../../../../subdifferential.md) is the set of supporting slopes

$$
\boxed{\partial f(x)=\{p\in\mathbb R^n:f(u)\geq f(x)+\langle p,u-x\rangle\ \text{for every }u\in\mathbb R^n\}}.
$$

Each element is a [subgradient](../../../../../../subgradient.md). Define $\partial f(x)=\varnothing$ outside $\operatorname{dom}f$. The defining [subgradient inequality](../../../../../../subgradient-inequality.md) must hold globally, not merely in a neighborhood of $x$. For a differentiable finite [convex function](../../../../../../convex-function.md), $\partial f(x)=\{\nabla f(x)\}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
