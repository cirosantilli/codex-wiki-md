<h1 id="3/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The noise has the product [Laplace distribution](../../../../../../../laplace-distribution.md) density

$$
g(y)=\prod_{j=1}^ke^{-2|y_j|}=e^{-2\|y\|_1},
$$

which is normalized because $\int_{\mathbb R}e^{-2|t|}\,dt=1$. By translation invariance of [Lebesgue measure](../../../../../../../lebesgue-measure.md), the conditional law of $A(u)+N$ has density

$$
p(y\mid u)=g(y-A(u))
=\exp[-2\|y-A(u)\|_1].
$$

Hence an associated [likelihood function](../../../../../../../likelihood-function.md) is

$$
\boxed{L(u;y)=\exp[-2\|y-A(u)\|_1]}.
$$

The map $(u,y)\mapsto y-A(u)$ is measurable because $A$ is measurable and vector subtraction is [continuous](../../../../../../../continuous-function.md). Composition with the continuous norm and exponential functions proves that $L$ is jointly measurable.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
