<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $q_0$ be the [stationary point](../../../../../../stationary-point.md) and let $H=D^2\beta(q_0)$ be its real symmetric [Hessian matrix](../../../../../../hessian-matrix.md). First suppose the [stationary point](../../../../../../stationary-point.md) is interior and nondegenerate, the [oscillatory integral amplitude](../../../../../../amplitude-of-an-oscillatory-integral.md) and [oscillatory integral phase](../../../../../../oscillatory-integral-phase.md) are sufficiently smooth, and boundary contributions are absent or smaller than the stationary contribution. Diagonalize $H$ by an orthogonal change of coordinates, with [eigenvalues](../../../../../../eigenvalue.md) $h_1,h_2$. Locally,

$$
\beta(q_0+\xi)=\beta(q_0)+\tfrac12\xi^TH\xi+O(|\xi|^3).
$$

Scaling each principal coordinate by $\lambda^{-1/2}$ and evaluating its [Fresnel integral](../../../../../../fresnel-integral.md) gives the [two-dimensional stationary-phase formula](../../../../../../two-dimensional-stationary-phase-formula.md):

$$
\boxed{h(\lambda)\sim\frac{2\pi}{\lambda}
\frac{\alpha(q_0)}{\sqrt{|\det H|}}
\exp\!\left(i\lambda\beta(q_0)+\frac{i\pi}4\operatorname{sgn}H\right).}
$$

Here $\operatorname{sgn}H$ is the number of positive [eigenvalues](../../../../../../eigenvalue.md) minus the number of negative ones: $2$, $0$ or $-2$. The formula gives the leading nonzero term when $\alpha(q_0)\ne0$. A [partition of unity](../../../../../../partition-of-unity.md) isolates this neighbourhood; [integration by parts](../../../../../../integration-by-parts.md) away from [stationary points](../../../../../../stationary-point.md) makes the remaining interior contribution smaller. For a smooth compactly supported [oscillatory integral amplitude](../../../../../../amplitude-of-an-oscillatory-integral.md) the local error is $O(\lambda^{-2})$.

The printed assumption of a single [stationary point](../../../../../../stationary-point.md) alone is insufficient for an unconditional answer. A degenerate [oscillatory integral phase](../../../../../../oscillatory-integral-phase.md) $\beta=x^4+y^2$ with a smooth [oscillatory integral amplitude](../../../../../../amplitude-of-an-oscillatory-integral.md) supported near the origin has only one [stationary point](../../../../../../stationary-point.md), but scales as $\lambda^{-3/4}$. Boundary terms can also contribute at order $\lambda^{-1}$: on the unit disk with [oscillatory integral amplitude](../../../../../../amplitude-of-an-oscillatory-integral.md) one and $\beta=x^2+y^2$,

$$
h(\lambda)=\frac{\pi(e^{i\lambda}-1)}{i\lambda},
$$

whose stationary contribution is $i\pi/\lambda$ and whose boundary contribution is $-i\pi e^{i\lambda}/\lambda$. Thus **the boxed formula is the standard nondegenerate interior stationary contribution**, with the stated hypotheses; the data as printed do not determine all possible leading behaviours.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
