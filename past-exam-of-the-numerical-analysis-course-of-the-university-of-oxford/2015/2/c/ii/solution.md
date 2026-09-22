<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The remainder in part (b) involves an unspecified $\xi=\xi(x)$. Its existence for every $x$ does not ensure a differentiable selection. Even if such a selection existed and $f$ had an additional [derivative](../../../../../derivative.md), the [product rule](../../../../../product-rule.md) and [chain rule](../../../../../chain-rule.md) would give

$$
\frac{d}{dx}\left[\frac{f^{(n+1)}(\xi(x))}{(n+1)!}\omega(x)\right]
=\frac{f^{(n+2)}(\xi(x))\xi'(x)\omega(x)+f^{(n+1)}(\xi(x))\omega'(x)}{(n+1)!}.
$$

The first term cannot be discarded or bounded from the given information. Neither $f^{(n+2)}$ nor $\xi'$ is supplied by the original theorem.

For an explicit demonstration, interpolate the [cubic polynomial](../../../../../cubic-polynomial.md) $f(x)=x^3$ at zero and one. Then $p_1(x)=x$, and

$$
f(x)-p_1(x)=x^3-x=(x+1)x(x-1).
$$

Differentiating correctly gives

$$
f'(x)-p_1'(x)=x(x-1)+(x+1)(2x-1)=3x^2-1.
$$

Treating the remainder coefficient $x+1$ as a constant would omit $x(x-1)$ and give a wrong answer at every interior point. **An existential intermediate point cannot be frozen when differentiating.** Part (i) instead applies [Rolle's theorem](../../../../../rolle-theorem.md) directly to the [polynomial interpolation error](../../../../../polynomial-interpolation-error.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
