<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [steady state](../../../../../../steady-state.md) is attractive here if every physical initial [density operator](../../../../../../density-matrix.md) approaches it. Subtracting its [Affine Bloch equation](../../../../../../affine-bloch-equation.md) from the trajectory equation gives $\delta\dot s=A\delta s$, so $\delta s(t)=e^{At}\delta s(0)$. The necessary and sufficient condition is

$$
\boxed{\operatorname{Re}\lambda<0\quad\text{for every eigenvalue }\lambda\text{ of }A}.
$$

Such an $A$ is a [Hurwitz stable matrix](../../../../../../hurwitz-stable-matrix.md). To prove sufficiency without assuming diagonalizability, put it in [Jordan normal form](../../../../../../jordan-normal-form.md). Each [Jordan block](../../../../../../jordan-block.md) contributes $e^{\lambda t}\sum_{j=0}^{q-1}t^jN^j/j!$, and the negative real part makes the exponential dominate all polynomial factors. For necessity, an eigenmode with positive real part grows; an eigenmode with zero real part remains constant or oscillates, so it does not tend to zero. A nontrivial Jordan block on the imaginary axis also prevents decay.

The physical [Bloch vector](../../../../../../bloch-vector.md) body has nonempty interior, so differences of physical initial vectors from $s_*$ span the full real coordinate space. Thus convergence for every physical initial state also forces $e^{At}\to0$ on that space. This rules out hiding a nondecaying eigenmode outside the physical set. The strict spectral condition entails uniqueness and global [asymptotic stability](../../../../../../asymptotic-stability.md) of the [steady state](../../../../../../steady-state.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
