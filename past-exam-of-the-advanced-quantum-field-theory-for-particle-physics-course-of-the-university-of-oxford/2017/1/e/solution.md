<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First remove the [projector](../../../../projection-linear-algebra.md) denominator explicitly:

$$
i\Pi_{\mathrm{ex}}=4e^2\mu^\epsilon\int\frac{d^dl}{(2\pi)^d}\frac{l^2k^2-(l\cdot k)^2}{(l^2)^2[(l+k)^2+m^2]}.
$$

Let $A=(l+k)^2+m^2$ and $B=l^2$. The [Feynman parameter for a simple and a squared propagator](../../../../feynman-parameter-for-a-simple-and-a-squared-propagator.md) follows by differentiating the elementary two-denominator [Feynman formula](../../../../feynman-parameter.md) with respect to $B$ gives

$$
\boxed{\frac1{AB^2}=2\int_0^1dx\frac{1-x}{[xA+(1-x)B]^3}.}
$$

Shift $q=l+xk$. Then $xA+(1-x)B=q^2+D$, with $D=x(1-x)k^2+xm^2$. The numerator is unchanged by this parallel shift:

$$
l^2k^2-(l\cdot k)^2=q^2k^2-(q\cdot k)^2.
$$

Therefore the correctly combined integral is

$$
\boxed{i\Pi_{\mathrm{ex}}=8e^2\mu^\epsilon\int_0^1(1-x)dx\int\frac{d^dq}{(2\pi)^d}\frac{q^2k^2-(q\cdot k)^2}{(q^2+D)^3}.}
$$

**The printed weight $x/2$ is not compatible with this denominator and prefactor.** Exchanging $x$ with $1-x$ changes the [mass term](../../../../mass.md) in $D$ as well and cannot supply the missing [normalization](../../../../normalization.md). A concrete counterexample is $m=0$ with nonzero spacelike [external momentum](../../../../four-momentum.md) and $2<d<4$: after [Wick rotation](../../../../wick-rotation.md), the remaining integral is nonzero and symmetric under $x\leftrightarrow1-x$. The source's $4e^2\int(x/2)dx$ expression is then exactly one quarter of the correct expression. Thus the claimed equality cannot be imposed when computing the pole.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
