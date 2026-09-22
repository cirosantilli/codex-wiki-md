<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The first observation has $x=(1,0,0)^T$ and one-hot label $y=(0,1)^T$ in the output order $(\mathrm{no},\mathrm{yes})$. If every kernel weight and bias initially equals one, each hidden preactivation is two, so $h=(2,2)^T$. Both logits equal five and $p=(1/2,1/2)^T$.

For [stochastic gradient descent](../../../../../../stochastic-gradient-descent.md) on one cross-entropy observation,

$$
\frac{\partial L}{\partial z}=p-y=(1/2,-1/2)^T.
$$

Hence the output-weight gradient has first row $(1,1)$ and second row $(-1,-1)$, while the output-bias gradient is $(1/2,-1/2)$. With learning rate one,

$$
V^{\mathrm{new}}=
\begin{pmatrix}0&0\\2&2\end{pmatrix},
\qquad
c^{\mathrm{new}}=(1/2,3/2)^T.
$$

Using the old output weights for backpropagation gives

$$
V^T(p-y)=(0,0)^T,
$$

so every entry of $W$ and $b$ remains equal to one after this batch.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
