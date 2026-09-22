<h1 id="question-2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the [divergence theorem](../../../../../../../divergence-theorem.md) to $\phi\mathbf c$, using [ii](../ii.md). Because the [vector](../../../../../../../vector.md) $\mathbf c$ is constant, it can be taken outside both [integrals](../../../../../../../integral-split.md):

$$
\mathbf c\cdot\iiint_V\nabla\phi\,dV
=\iiint_V\nabla\cdot(\phi\mathbf c)\,dV
=\iint_{\partial V}\phi\mathbf c\cdot\mathbf n\,dS
=\mathbf c\cdot\iint_{\partial V}\phi\mathbf n\,dS.
$$

This holds for every $\mathbf c$, in particular each of the three Cartesian [basis vectors](../../../../../../../basis-vector.md). Equality of the three components proves the [gradient volume-to-boundary identity](../../../../../../../gradient-volume-to-boundary-identity.md)

$$
\boxed{\iiint_V\nabla\phi\,dV=\iint_{\partial V}\phi\mathbf n\,dS.}
$$

It suffices that $\phi$ be a [continuously differentiable function](../../../../../../../continuously-differentiable-function.md) on a neighbourhood of the [closure](../../../../../../../closure-topology.md) of $V$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [Question 2](../../../question-2.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
