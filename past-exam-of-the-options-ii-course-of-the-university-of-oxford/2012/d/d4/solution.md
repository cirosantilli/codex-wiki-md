<h1 id="d/d4/solution">Solution</h1>

↑ **Parent:** [D4](../d4.md)

For a [continuously differentiable](../../../../continuously-differentiable-function.md) [diffeomorphism](../../../../diffeomorphism.md) $\phi:J\to I$ between [intervals](../../../../interval-mathematics.md), the [integration by substitution](../../../../integration-by-substitution.md) states

$$
\int_I h(x)\,dx=\int_J h(\phi(t))|\phi'(t)|\,dt.
$$

It holds as an [identity element](../../../../identity-element.md) of extended [integrals](../../../../integral-split.md) for nonnegative [measurable](../../../../measurability.md) $h$. For signed or complex-valued [measurable](../../../../measurability.md) $h$, [integrability](../../../../integrability.md) on one side is equivalent to [integrability](../../../../integrability.md) after [substitution](../../../../substitution-algebra.md), and the [identity element](../../../../identity-element.md) then holds. The absolute [derivative](../../../../derivative.md) accounts for a decreasing [substitution](../../../../substitution-algebra.md); on oriented finite [intervals](../../../../interval-mathematics.md) the equivalent formula uses $\phi'$ and oriented endpoints.

Put $C=\int_0^\infty(1+x^4)^{-1}\,dx=\pi/(2\sqrt2)$. The map $x=y^{-1/4}$ is a decreasing [diffeomorphism](../../../../diffeomorphism.md) of the positive half-line onto itself and

$$
\frac{|dx/dy|}{1+x^4}=\frac1{4y^{1/4}(1+y)}.
$$

Applying the nonnegative version before assuming finiteness proves both existence and value:

$$
\boxed{\int_0^\infty\frac{dy}{y^{1/4}(1+y)}=4C=\sqrt2\pi.}
$$

[Tonelli's theorem](../../../../tonelli-theorem.md) permits either iterated [integral](../../../../integral-split.md) of a nonnegative [measurable function](../../../../measurable-function.md) on a product of sigma-finite [measure spaces](../../../../measure-space.md) and identifies both with its extended product [integral](../../../../integral-split.md). [Fubini's theorem](../../../../fubini-s-theorem.md) states that for an absolutely [integrable](../../../../integrability.md) [measurable function](../../../../measurable-function.md) on such a product, almost every section is [integrable](../../../../integrability.md), the section-integral functions are [integrable](../../../../integrability.md), and the two iterated [integrals](../../../../integral-split.md) equal the product [integral](../../../../integral-split.md).

The given two-variable function is [continuous](../../../../continuous-function.md) and positive on the positive quadrant. For fixed $y>0$, substituting $t=xy^{1/4}$ gives

$$
\int_0^\infty f(x,y)\,dx=\frac{Cy^{-1/4}}{1+y}.
$$

Tonelli now gives

$$
\iint f(x,y)\,dx\,dy=C(4C)=4C^2=\frac{\pi^2}2<\infty.
$$

This proves [absolute integrability](../../../../integrability.md), so Fubini is applicable.

For $x\neq1$, integrate the displayed partial fraction [identity element](../../../../identity-element.md) in $y$ up to $R$:

$$
\int_0^R f(x,y)\,dy=\frac{\log(1+x^4R)-\log(1+R)}{x^4-1}
\longrightarrow\frac{4\log x}{x^4-1}.
$$

At $x=1$ the section [integral](../../../../integral-split.md) is $\int_0^\infty(1+y)^{-2}\,dy=1$, agreeing with the [continuous](../../../../continuous-function.md) limit of this expression. Therefore Fubini identifies the remaining [integral](../../../../integral-split.md) and gives

$$
\boxed{\int_0^\infty\frac{\log x}{x^4-1}\,dx=\frac14\cdot\frac{\pi^2}2=\frac{\pi^2}8.}
$$

The apparent [singularity](../../../../complex-singularity.md) at one is removable, with limiting integrand value $1/4$. Positivity and the finite product [integral](../../../../integral-split.md) already establish convergence at both ends.

## ↑ Ancestors (12)

1. [D4](../d4.md)
2. [D](../../d.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
