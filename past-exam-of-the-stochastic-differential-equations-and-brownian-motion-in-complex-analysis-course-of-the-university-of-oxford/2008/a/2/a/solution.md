<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [drift coefficient](../../../../../drift-coefficient.md) $b(z)=rz$ and [diffusion coefficient](../../../../../diffusion-coefficient.md) $a(z)=\sigma z$ are [Lipschitz continuity](../../../../../lipschitz-continuity.md) and have linear growth. The standard existence and [pathwise uniqueness](../../../../../pathwise-uniqueness.md) theorem for [stochastic differential equations](../../../../../stochastic-differential-equation.md) therefore supplies a unique global [strong solution of a stochastic differential equation](../../../../../strong-solution-of-a-stochastic-differential-equation.md), adapted to the driving [Brownian filtration](../../../../../brownian-filtration.md).

Apply [Itô's formula](../../../../../ito-s-lemma.md) to $x\exp((r-\sigma^2/2)t+\sigma B_t)$. Its time derivative contributes $(r-\sigma^2/2)X_t$ and its Itô correction contributes $\sigma^2X_t/2$, giving the required equation and initial value. Hence

$$
\boxed{X_t=x e^{(r-\sigma^2/2)t+\sigma B_t}.}
$$

In particular the solution stays positive. For $t>s$, factor out $X_s$ and use [independence](../../../../../independent-random-variables.md) and the normal law of $B_t-B_s$:

$$
\boxed{\mathbb E(X_t\mid\mathcal F_s^0)
=e^{r(t-s)}X_s.}
$$

The exponential moment exists, so this [conditional expectation](../../../../../conditional-expectation.md) is well-defined for every finite $s,t$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
