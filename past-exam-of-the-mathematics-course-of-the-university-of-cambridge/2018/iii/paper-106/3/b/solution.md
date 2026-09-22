<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the [Riesz-Markov-Kakutani representation theorem](../../../../../../riesz-markov-kakutani-representation-theorem.md), the [continuous dual space](../../../../../../continuous-dual-space-split.md) of $C(K)$ is isometrically the space of finite [regular Borel measures](../../../../../../regular-borel-measure.md), signed for real scalars and complex for complex scalars:

$$
\boxed{C(K)^*\cong M(K),\qquad L_\mu(f)=\int_Kf\,d\mu,\qquad \|L_\mu\|=|\mu|(K).}
$$

Here $|\mu|$ is the [variation measure](../../../../../../variation-measure.md), whose total mass is the [total variation norm of a measure](../../../../../../total-variation-norm-of-a-measure.md).

If $f_n\rightharpoonup0$ in $C(K)$, evaluation at each $t\in K$ gives $f_n(t)\to0$. The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) also gives $M=\sup_n\|f_n\|_\infty<\infty$. For any $\mu\in M(K)$, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) with respect to the finite positive measure $|\mu|$ yields

$$
\left|\int_Kf_n^2\,d\mu\right|\leq\int_K|f_n|^2\,d|\mu|\longrightarrow0,
$$

since $|f_n(t)|^2\to0$ pointwise and $|f_n(t)|^2\leq M^2$. Thus

$$
\boxed{f_n^2\rightharpoonup0\text{ in }C(K).}
$$

The same proof works for complex squares, because the absolute-value domination remains valid.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
