<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix the measure conventions before evaluating this [zero-dimensional supersymmetric field theory](../../../../../../zero-dimensional-supersymmetric-field-theory.md). Take $dz\,d\bar z$ to mean ordinary positive area measure $d^2z=dx\,dy$, and choose [Berezin integration](../../../../../../berezin-integral.md) orientations with $\int d^2\theta\,\theta_1\theta_2=\int d^2\overline\theta\,\overline\theta_1\overline\theta_2=1$. A different overall measure normalization multiplies all the unnormalized answers by the same constant. Assume $r=\deg P=\deg W-1\ge1$, so $|P(z)|\to\infty$ at infinity and all polynomial insertions converge. An affine or constant $W$ does not give this confining integral and is outside this convergence hypothesis.

The [Grassmann variables](../../../../../../grassmann-variable.md) truncate the fermionic exponential. The coefficient of $\theta_1\theta_2\overline\theta_1\overline\theta_2$ is $P'(z)\overline{P'(z)}$, so the [partition function](../../../../../../canonical-partition-function.md) becomes

$$
Z=\int_{\mathbb C}d^2z\,|P'(z)|^2e^{-|P(z)|^2}.
$$

The [Jacobian determinant](../../../../../../jacobian-determinant.md) of the [holomorphic map](../../../../../../holomorphic-map.md) $w=P(z)$ is $|P'(z)|^2$. Away from its finitely many critical values, a polynomial of [polynomial degree](../../../../../../degree-of-a-polynomial.md) $r$ has $r$ preimages counted with multiplicity. The [change of variables formula](../../../../../../change-of-variables-formula.md) therefore gives

$$
\boxed{Z=r\int_{\mathbb C}d^2w\,e^{-|w|^2}=\pi r=\pi(\deg W-1).}
$$

Critical values form a set of area zero and do not affect the integral. This [partition function](../../../../../../canonical-partition-function.md) measures the covering degree, even when some zeros of $P$ are repeated.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
