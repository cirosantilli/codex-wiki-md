<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a real [scalar field](../../../../../../scalar-field.md) and Minkowski [action](../../../../../../action.md) $S[\phi]$, with the vacuum selected by a [Feynman propagator](../../../../../../feynman-propagator.md) pole prescription or adiabatic vacuum boundary conditions. The normalized [correlation functions](../../../../../../correlation-function.md) are

$$
G_n(x_1,\ldots,x_n)=\frac{\int\mathcal D\phi\,\phi(x_1)\cdots\phi(x_n)e^{iS[\phi]}}{\int\mathcal D\phi\,e^{iS[\phi]}}=\langle\Omega|\mathcal T\{\widehat\phi_H(x_1)\cdots\widehat\phi_H(x_n)\}|\Omega\rangle.
$$

Here $|\Omega\rangle$ is the interacting vacuum and $\mathcal T$ denotes [time ordering](../../../../../../time-ordering.md). These are the canonical [vacuum expectation values](../../../../../../vacuum-expectation-value.md), rather than unordered products of noncommuting fields. The [functional integral](../../../../../../functional-measure.md) formula assumes a regulated measure and the same vacuum prescription on both sides.

Couple an [external source](../../../../../../source-quantum-field-theory.md) $J$ linearly to the [scalar field](../../../../../../scalar-field.md) and choose the [normalized vacuum generating functional](../../../../../../normalized-vacuum-generating-functional.md)

$$
Z[J]=\frac{\int\mathcal D\phi\,\exp\left(iS[\phi]+i\int d^dx\,J\phi\right)}{\int\mathcal D\phi\,e^{iS[\phi]}},\qquad Z[0]=1.
$$

Then [functional derivatives](../../../../../../functional-derivative.md) insert the fields:

$$
G_n=\left.i^{-n}\frac{\delta^nZ}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0},\qquad Z[J]=\sum_{n=0}^\infty\frac{i^n}{n!}\int G_n(x_1,\ldots,x_n)\prod_{j=1}^n J(x_j)\,d^dx_j.
$$

In the convention used below, the [connected generating functional](../../../../../../connected-generating-functional.md) is

$$
\boxed{Z[J]=e^{iW[J]},\qquad W[J]=-i\log Z[J],\qquad G_n^c=\left.i^{1-n}\frac{\delta^nW}{\delta J(x_1)\cdots\delta J(x_n)}\right|_{J=0}.}
$$

The logarithm removes products of disconnected components. For example the [connected correlation function](../../../../../../connected-correlation-function.md) $G_2^c=G_2-G_1G_1$; at three points one subtracts all three $G_2G_1$ products and adds $2G_1G_1G_1$. Normalization has already removed [vacuum bubbles](../../../../../../vacuum-feynman-diagram.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
