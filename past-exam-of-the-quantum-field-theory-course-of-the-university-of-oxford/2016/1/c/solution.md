<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First take the [trace](../../../../matrix-trace.md) in four [spacetime](../../../../spacetime.md) dimensions:

$$
T^\mu{}_{\mu}=-(\partial\phi)^2+2m^2\phi^2+\frac{\lambda}{6}\phi^4,
\qquad
\Omega^\mu{}_{\mu}=T^\mu{}_{\mu}-3C\Box\phi^2.
$$

The [product rule](../../../../product-rule.md) gives $\Box\phi^2=2(\partial\phi)^2+2\phi\Box\phi$. For the massless [equation of motion](../../../../equation-of-motion.md), $\phi\Box\phi=-\lambda\phi^4/6$, so

$$
\left.\Omega^\mu{}_{\mu}\right|_{F=0,m=0}
=-(1+6C)(\partial\phi)^2+\lambda\left(\frac16+C\right)\phi^4.
$$

Both coefficients vanish for

$$
\boxed{C=-\frac16.}
$$

The minus sign follows from the order $\partial^\mu\partial^\nu-\eta^{\mu\nu}\Box$ used in the question's [stress-energy tensor improvement](../../../../stress-energy-tensor-improvement.md). Commuting [partial derivatives](../../../../partial-derivative.md) shows that this improvement has identically zero [divergence](../../../../divergence.md), so it preserves the conservation law.

The precise [trace](../../../../matrix-trace.md) identity, without using the [equation of motion](../../../../equation-of-motion.md), is

$$
\boxed{\Omega^\mu{}_{\mu}=m^2\phi^2+\phi F.}
$$

Hence the massless [tensor](../../../../tensor.md) is traceless **on shell**. It is not traceless for arbitrary [off shell](../../../../off-shell.md) configurations: a nonzero constant $\phi=A$ with $\lambda\ne0$ has $\Omega^\mu{}_{\mu}=\lambda A^4/6$. This is a classical result; it does not assert absence of a quantum [trace anomaly](../../../../trace-anomaly.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
