<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each map $x\mapsto\langle a_i,x\rangle+b_i$ is an [affine function](../../../../../../affine-function.md). For $0\leq t\leq1$, the [pointwise maximum of convex functions](../../../../../../pointwise-maximum-of-convex-functions.md) satisfies

$$
\begin{aligned}
f(tx+(1-t)y)
&=\max_i\{t(\langle a_i,x\rangle+b_i)+(1-t)(\langle a_i,y\rangle+b_i)\}\\
&\leq t f(x)+(1-t)f(y),
\end{aligned}
$$

so $f$ is [convex](../../../../../../convex-function.md).

A vector $g$ is a [subgradient](../../../../../../subgradient.md) of a [convex function](../../../../../../convex-function.md) $f$ at $x$ when

$$
f(y)\geq f(x)+\langle g,y-x\rangle
$$

for every $y$. Choose any active index $j\in I(x):=\{i:f(x)=\langle a_i,x\rangle+b_i\}$. Then

$$
f(y)\geq\langle a_j,y\rangle+b_j
=f(x)+\langle a_j,y-x\rangle,
$$

and hence $\boxed{a_j\in\partial f(x)}$. More generally, every [convex combination](../../../../../../convex-combination.md) of the active vectors is a subgradient, and in fact

$$
\boxed{\partial f(x)=\operatorname{conv}\{a_i:i\in I(x)\}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
