<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Yes: for $k=2$ the stated inequality guarantees [zero-stability](../../../../../zero-stability.md).** Part (ii) puts every [polynomial root](../../../../../root-of-a-polynomial.md) in the closed [unit disc](../../../../../unit-disc.md). The remaining [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) is that every root on the [unit circle](../../../../../complex-unit-circle.md) has [multiplicity of a root](../../../../../multiplicity-of-a-root.md) one.

If this failed for a [quadratic polynomial](../../../../../quadratic-polynomial.md), it would have a repeated root $\xi$ with $|\xi|=1$, and

$$
\rho(z)=\alpha_2(z-\xi)^2
=\alpha_2z^2-2\alpha_2\xi z+\alpha_2\xi^2.
$$

Consequently $|\alpha_1|=2|\alpha_2|$ and $|\alpha_0|=|\alpha_2|$, contradicting

$$
|\alpha_2|\geq|\alpha_0|+|\alpha_1|=3|\alpha_2|,
$$

because $\alpha_2\ne0$. Thus all roots on the [unit circle](../../../../../complex-unit-circle.md) are simple and

$$
\boxed{\text{The method is zero-stable; no counterexample satisfies the assumption.}}
$$

This conclusion does not assert [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md): part (i) rules out [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) whenever the coefficient inequality is strict. [Zero-stability](../../../../../zero-stability.md) and [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) are separate requirements.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
