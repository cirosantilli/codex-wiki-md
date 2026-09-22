<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [local Maxwellian](../../../../../../local-maxwellian.md) can be written as $\mathcal M=\exp(a+b\cdot v+c|v|^2)$, with $c<0$ and coefficients depending on $(t,x)$. Its logarithm is a [linear combination](../../../../../../linear-combination.md) of [collision invariants](../../../../../../collision-invariant.md), so $\mathcal M'\mathcal M_*'=\mathcal M\mathcal M_*$ and $Q(\mathcal M,\mathcal M)=0$ at each spatial point.

Comparing powers of $v$ in $(\partial_t+v\cdot\nabla_x)\log\mathcal M=0$ gives

$$
\nabla_xc=0,\qquad\operatorname{sym}\nabla_xb+c_tI_3=0,\qquad b_t+\nabla_xa=0,\qquad a_t=0.
$$

Here $\operatorname{sym}\nabla b$ is the [symmetric part of a matrix](../../../../../../symmetric-part-of-a-matrix.md) formed by the coefficients of the quadratic polynomial. For constants $A,\alpha,\beta>0$, choose $a=\log A-\alpha|x|^2$, $b=2\alpha tx$ and $c=-\beta-\alpha t^2$. All four coefficient equations hold. The resulting [expanding Gaussian solution of the Boltzmann equation](../../../../../../expanding-gaussian-solution-of-the-boltzmann-equation.md) is

$$
\boxed{f(t,x,v)=A\exp\bigl(-\alpha|x-tv|^2-\beta|v|^2\bigr)}.
$$

Direct verification is particularly simple: $x-tv$ and $v$ are constant along free [characteristic curves](../../../../../../characteristic-curve.md), so the transport [derivative](../../../../../../derivative.md) is zero. At fixed $(t,x)$ its logarithm is the displayed [Maxwellian](../../../../../../local-maxwellian.md) quadratic, so the collision term is also zero. Its spatial dependence is nonconstant, it is positive and rapidly decaying, and its Gaussian velocity [integral](../../../../../../integral.md) is finite because $\beta+\alpha t^2>0$. It is not a compactly supported example, nor does this final part require one.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
