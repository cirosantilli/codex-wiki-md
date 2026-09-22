<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Insert the [travelling wave](../../../../../../../travelling-wave.md) into the [viscous scalar conservation law](../../../../../../../viscous-scalar-conservation-law.md). With $s=x-\sigma t$ the equation becomes

$$
-\sigma v'+F'(v)v'=\varepsilon v'',
$$

and one integration gives

$$
\varepsilon v'=F(v)-\sigma v+b=:Q(v).
$$

For a nonconstant profile, $Q(v(s))$ never vanishes. Indeed, the autonomous [ordinary differential equation](../../../../../../../ordinary-differential-equation.md) $v'=Q(v)/\varepsilon$ has unique local solutions since $Q$ is $C^1$; reaching an equilibrium would force the whole solution to be constant. Separation and $c=v(0)$ therefore give

$$
\boxed{s=\int_c^{v(s)}\frac{\varepsilon}{F(z)-\sigma z+b}\,dz.}
$$

A different choice of reference point gives $s-s_0$ on the left, expressing the translation freedom of the [travelling wave](../../../../../../../travelling-wave.md).

**The printed formula needs a nonconstant-profile qualification.** Constant profiles also solve the PDE, but their denominator vanishes at their constant value, so the separated integral is not defined. They must be included separately as equilibrium solutions of the integrated [ordinary differential equation](../../../../../../../ordinary-differential-equation.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
