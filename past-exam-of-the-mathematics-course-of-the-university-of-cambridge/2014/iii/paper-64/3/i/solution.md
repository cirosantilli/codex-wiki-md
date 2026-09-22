<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [structure theorem for functions of bounded variation](../../../../../../structure-theorem-for-functions-of-bounded-variation.md) is the [measure](../../../../../../measure.md) representation of the [distributional derivative](../../../../../../distributional-derivative.md): for $u\in BV(\Omega)$ there is a unique finite [vector Radon measure](../../../../../../vector-radon-measure.md) $Du$ with

$$
\boxed{\int_\Omega u\,\operatorname{div}\varphi\,dx=-\int_\Omega\varphi\cdot dDu,\qquad |Du|(\Omega)=\operatorname{TV}(u)}
$$

for every $\varphi\in C_c^1(\Omega;\mathbb R^n)$. It also has a [polar decomposition of a vector measure](../../../../../../polar-decomposition-of-a-vector-measure.md) $Du=\sigma_u|Du|$ with $|\sigma_u|=1$ for $|Du|$-almost every point.

To prove it, let $L(\varphi)=-\int u\operatorname{div}\varphi$. The test-function definition of [total variation seminorm](../../../../../../total-variation-seminorm-on-a-domain.md), applied to both signs, gives $|L(\varphi)|\le\operatorname{TV}(u)\|\varphi\|_\infty$. Compactly supported smooth [vector fields](../../../../../../vector-field.md) are uniformly dense in $C_0(\Omega;\mathbb R^n)$, so $L$ extends uniquely to a bounded functional there. The [Riesz-Markov-Kakutani representation theorem](../../../../../../riesz-markov-kakutani-representation-theorem.md), applied componentwise, gives the unique [vector measure](../../../../../../vector-measure.md) $Du$. The operator [norm](../../../../../../norm.md) of $L$ is exactly the defining variation supremum; the vector-measure dual [norm](../../../../../../norm.md) is $|Du|(\Omega)$, proving equality. Conversely any [finite measure](../../../../../../finite-measure.md) satisfying the identity bounds that supremum, so this also characterizes membership in the [BV space](../../../../../../function-of-bounded-variation-on-a-domain.md).

The [Radon-Nikodym theorem](../../../../../../radon-nikodym-theorem.md) applied to the components relative to $|Du|$ gives $\sigma_u$; the definition of the [variation measure](../../../../../../variation-measure.md) forces $|\sigma_u|=1$ [almost everywhere](../../../../../../almost-everywhere.md). If $u$ is smooth, ordinary [integration by parts](../../../../../../integration-by-parts.md) gives $Du=\nabla u\,\mathcal L^n$. [Compact support](../../../../../../compact-support.md) of the test field removes any boundary contribution; no boundary regularity is needed for this representation statement.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
