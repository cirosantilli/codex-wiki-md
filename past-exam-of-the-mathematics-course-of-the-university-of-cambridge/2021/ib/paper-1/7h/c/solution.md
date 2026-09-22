<h1 id="7h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [softplus function](../../../../../../softplus.md)

$$
h(s)=\log(1+e^s)
$$

is convex because

$$
h''(s)=\frac{e^s}{(1+e^s)^2}\geq0.
$$

Part (b) therefore shows that every $\beta\mapsto h(a_i^T\beta)$ is convex. The [absolute value function](../../../../../../absolute-value.md) is convex, so $\beta\mapsto|\beta_j|$ is convex for every coordinate $j$. Finally, part (a) says that a finite sum of convex functions is convex. Therefore

$$
Q(\beta)=\sum_{i=1}^n\log(1+e^{a_i^T\beta})+\sum_{j=1}^d|\beta_j|
$$

is convex. The second sum is the [L1 norm](../../../../../../l1-norm.md) regularizer.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
