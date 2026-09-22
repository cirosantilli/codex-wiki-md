<h1 id="2/iii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use decaying variations with the same complex bulk field one, so that [integration by parts](../../../../../../../integration-by-parts.md) produces no variation boundary term. The [functional derivatives](../../../../../../../functional-derivative.md) of energy and [renormalized momentum of a condensate](../../../../../../../renormalized-momentum-of-a-condensate.md) are

$$
\frac{\delta E}{\delta\psi^*}=-\frac12\left[\nabla^2\psi+(1-|\psi|^2)\psi\right],\qquad
\frac{\delta p}{\delta\psi^*}=-i\partial_z\psi.
$$

For the second identity, variation of the two momentum terms and integration of the $\partial_z\delta\psi^*$ term each supply $(2i)^{-1}\psi_z$, so together they give $-i\psi_z$. It follows that

$$
\frac{\delta(E-Up)}{\delta\psi^*}=
-\frac12\left[\nabla^2\psi+(1-|\psi|^2)\psi\right]+iU\psi_z=0
$$

is exactly the stationary [Gross–Pitaevskii solitary wave](../../../../../../../gross-pitaevskii-solitary-wave.md) equation. Thus each solitary wave is a constrained energy critical point with multiplier $U$.

Let $s$ parametrize a differentiable family of these waves. Apply the critical-point identity to the variation $\partial_s\psi$, keeping the multiplier fixed at its value for that member of the family. Including the [complex conjugate](../../../../../../../complex-conjugate.md) variation gives

$$
\frac{dE}{ds}-U(s)\frac{dp}{ds}=0.
$$

Hence the [energy–momentum slope of a solitary wave](../../../../../../../energy-momentum-slope-of-a-solitary-wave.md) is

$$
\boxed{\frac{dE}{dp}=U}
$$

wherever $dp/ds\ne0$. At a momentum turning point the parametrized identity $dE/ds=U\,dp/ds$ remains the correct statement; a globally single-valued energy as a function of momentum is not needed. Differentiating $E-U(s)p$ as a composite function would include an extra $-pU'$ term, so that composite derivative must not be set to zero.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iii](../../iii.md)
3. [2](../../../2.md)
4. [Paper 84](../../../../paper-84-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
