<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an [edge](../../../../../../../edge-of-a-graph.md) $ij$, put $\rho=\langle v_i,v_j\rangle$ and $\theta=\arccos\rho$. Since $\rho\leq-1/2$, we have $\theta\geq2\pi/3$.

The random normal $a$ has the isotropic [Gaussian distribution](../../../../../../../normal-distribution.md) $N(0,I_p)$. Its distribution is invariant under [orthogonal transformations](../../../../../../../orthogonal-transformation.md); if $v_i,v_j$ are linearly independent, its projection onto their [plane](../../../../../../../plane.md) has a uniformly distributed direction. The signs of its [inner products](../../../../../../../inner-product.md) with $v_i,v_j$ differ in two sectors of total angle $2\theta$, out of $2\pi$. Thus [random hyperplane rounding](../../../../../../../random-hyperplane-rounding.md) gives

$$
\boxed{\mathbb P(H\text{ cuts }ij)=\frac{\theta}{\pi}\geq\frac23.}
$$

If $v_j=-v_i$, the signs differ with probability one and the same formula holds with $\theta=\pi$. Zero [inner products](../../../../../../../inner-product.md) have probability zero, since each $v_i$ is a [unit vector](../../../../../../../unit-vector.md).

If the [graph](../../../../../../../graph-split.md) has an [edge](../../../../../../../edge-of-a-graph.md), its corresponding principal $2\times2$ block of $U$ forces $t\geq2$, so the division by $t-1$ used to obtain the [Gram matrix](../../../../../../../gram-matrix.md) is valid. An edgeless [graph](../../../../../../../graph-split.md) can instead be colored with one color directly.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
