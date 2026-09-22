<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
\tau=\min\bigl(\{m\leq n:|S_m|>x\}\cup\{n\}\bigr).
$$

Because $|X_m|\leq K$, one always has $|S_\tau|\leq x+K$: this is clear if no crossing occurs, and at the first crossing the overshoot is at most one increment. Apply the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the martingale from part (c):

$$
\mathbb E[S_\tau^2]=\mathbb E[V_\tau]\leq(x+K)^2.
$$

On the event $\{\max_{m\leq n}|S_m|\leq x\}$ one has $\tau=n$, so $V_\tau=V_n$. Since $V_\tau\geq0$ everywhere,

$$
V_n\mathbb P\left(\max_{m\leq n}|S_m|\leq x\right)
\leq\mathbb E[V_\tau]
\leq(x+K)^2.
$$

Hence

$$
\boxed{\mathbb P\left(\max_{1\leq m\leq n}|S_m|\leq x\right)
\leq\frac{(x+K)^2}{\operatorname{Var}(S_n)}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
