<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Malgrange–Ehrenpreis theorem](../../../../../malgrange-ehrenpreis-theorem.md) states that every nonzero constant-coefficient [linear partial differential operator](../../../../../linear-partial-differential-operator.md) $P(D)$ on $\mathbb R^n$ has a [fundamental solution of a linear differential operator](../../../../../fundamental-solution-of-a-linear-differential-operator.md): there is an $E\in\mathcal D'(\mathbb R^n)$ such that $P(D)E=\delta_0$.

Write $D=-i\partial$. After an [orthogonal change of coordinates](../../../../../orthogonal-matrix.md) and multiplication by a nonzero constant, its polynomial symbol may be written as a monic polynomial in the last frequency,

$$
P(\xi',z)=z^M+\sum_{m=0}^{M-1}a_m(\xi')z^m.
$$

For each real $\mu'$, this polynomial has $M$ complex roots counted with multiplicity. Among a fixed finite collection of horizontal lines at bounded heights, one can choose a line that stays a positive distance from all those roots. Continuity of the roots preserves the choice on a neighborhood $N(\mu')$. Take a countable locally finite cover by such neighborhoods, refine it to a measurable disjoint partition $\mathbb R^{n-1}=\bigsqcup_j\Delta_j$, and let $c_j$ be the chosen height on $\Delta_j$. The resulting [Hörmander staircase](../../../../../hormander-staircase.md)

$$
\Sigma=\bigcup_j\{(\xi',s+ic_j):\xi'\in\Delta_j,\ s\in\mathbb R\}
$$

has bounded heights and may be chosen so that $|P(\xi',s+ic_j)|\geq1$ on each step.

For a [test function](../../../../../test-function.md) $\varphi$, define

$$
\langle E,\varphi\rangle
=\frac1{(2\pi)^n}\sum_j
\int_{\Delta_j}\int_{\mathbb R+ic_j}
\frac{\widehat\varphi(-\xi',-z)}{P(\xi',z)}\,dz\,d\xi'.
$$

The [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md) gives rapid decay in the real frequency directions and at most a fixed exponential factor in the bounded imaginary direction. Together with $|P|\geq1$, this proves that the integral defines a continuous [distribution](../../../../../distribution-mathematical-analysis.md). Applying $P(D)$ cancels the denominator. The remaining integrand is [entire](../../../../../entire-function.md) in $z$, so the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) shifts every horizontal contour to the real axis; the partition then recombines into $\mathbb R^{n-1}$. The [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) gives

$$
\langle P(D)E,\varphi\rangle=\varphi(0)=\langle\delta_0,\varphi\rangle,
$$

which proves the theorem.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
