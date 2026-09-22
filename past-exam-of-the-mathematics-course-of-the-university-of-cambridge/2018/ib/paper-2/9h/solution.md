<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

A function $f:\mathbb R^n\to\mathbb R$ is a [convex function](../../../../../convex-function.md) when

$$
f((1-t)x_0+tx_1)\leq(1-t)f(x_0)+tf(x_1)
$$

for every $x_0,x_1$ and $t\in[0,1]$.

Fix $b_0,b_1\in\mathbb R$, $t\in[0,1]$, and $\varepsilon>0$. Since the [value function](../../../../../value-function.md) is finite, choose $x_i$ with

$$
g(x_i)\leq b_i,
\qquad
f(x_i)\leq\phi(b_i)+\varepsilon.
$$

For the [convex combination](../../../../../convex-combination.md) $x_t=(1-t)x_0+tx_1$, convexity of $g$ gives

$$
g(x_t)\leq(1-t)b_0+tb_1,
$$

so $x_t$ is feasible for the intermediate right-hand side. Convexity of $f$ then gives

$$
\phi((1-t)b_0+tb_1)
\leq f(x_t)
\leq(1-t)\phi(b_0)+t\phi(b_1)+\varepsilon.
$$

Letting $\varepsilon\downarrow0$ proves

$$
\boxed{\phi((1-t)b_0+tb_1)\leq(1-t)\phi(b_0)+t\phi(b_1),}
$$

so **$\phi$ is convex.**

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
