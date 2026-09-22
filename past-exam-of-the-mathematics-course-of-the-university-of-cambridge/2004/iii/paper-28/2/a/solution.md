<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Finite [second moment](../../../../../../second-moment.md) implies $\mathbb EX<\infty$. For $\lambda$ near any positive $\lambda_0$, the [derivative](../../../../../../derivative.md) of $e^{-\lambda X}$ is bounded in absolute value by $X$, provided the neighbourhood stays in $(0,\infty)$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore permits [differentiation](../../../../../../differentiation.md) under the [expectation](../../../../../../expected-value.md):

$$
\boxed{\phi_X'(\lambda)=-\mathbb E[Xe^{-\lambda X}],\qquad\lambda>0.}
$$

For the expansion, put $r(z)=e^{-z}-1+z-z^2/2$. [Taylor expansion](../../../../../../taylor-expansion.md) gives $r(z)/z^2\to0$ as $z\downarrow0$. Also, for $z\geq0$,

$$
0\leq e^{-z}-1+z\leq\frac{z^2}{2},
\qquad |r(z)|\leq\frac{z^2}{2}.
$$

The inequalities follow by integrating $0\leq1-e^{-u}\leq u$ from zero to $z$. Consequently $r(\lambda X)/\lambda^2\to0$ pointwise and its absolute value is bounded by $X^2/2$. Another application of the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives the [second-moment expansion of a Laplace transform](../../../../../../second-moment-expansion-of-a-laplace-transform.md):

$$
\boxed{\phi_X(\lambda)=1-\lambda\mathbb EX
+\frac{\lambda^2}{2}\mathbb EX^2+o(\lambda^2),\qquad\lambda\downarrow0.}
$$

No third moment is needed for the remainder estimate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
