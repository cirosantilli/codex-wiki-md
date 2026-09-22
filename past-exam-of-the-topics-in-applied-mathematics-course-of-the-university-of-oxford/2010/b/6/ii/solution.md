<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) equation gives $y=x$, and the third gives $z=x^2/b$. The second then becomes $x(r-1-x^2/b)=0$. Hence the [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md) are

$$
\boxed{O=(0,0,0),\qquad C_\pm=(\pm\sqrt{b(r-1)},\pm\sqrt{b(r-1)},r-1)\quad(r>1).}
$$

At the origin, one [eigenvalue](../../../../../eigenvalue.md) is $-b$ and the remaining two solve $\lambda^2+(\sigma+1)\lambda+\sigma(1-r)=0$. Their discriminant is $(\sigma-1)^2+4\sigma r>0$. For $r<1$ both are negative, so the origin is [linearly stable](../../../../../linear-stability.md), with all [eigenvalues](../../../../../eigenvalue.md) real and negative. For $r>1$ one is positive and one negative, so it is a [saddle equilibrium](../../../../../saddle-equilibrium.md) with one unstable and two stable directions. At $r=1$ its [eigenvalues](../../../../../eigenvalue.md) are $0,-(\sigma+1),-b$: [linearization](../../../../../linearization.md) has a neutral direction and cannot alone prove nonlinear stability. Given the source's global attraction for $r<1$, there are no nontrivial [limit cycles](../../../../../limit-cycle.md) or persistent chaotic invariant dynamics in that regime; all initial states tend to the origin.

To establish the local pitchfork, one needs the simple [eigenvalue](../../../../../eigenvalue.md) to cross zero, the two symmetry-related branches to exist and acquire the expected local stability, and nondegeneracy of the nonlinear coefficient. The [derivative](../../../../../derivative.md) of the crossing [eigenvalue](../../../../../eigenvalue.md) is $\sigma/(\sigma+1)>0$. At $C_\pm$, the [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\boxed{\lambda^3+(\sigma+b+1)\lambda^2+b(\sigma+r)\lambda+2\sigma b(r-1)=0.}
$$

For $r>1$ sufficiently close to one, all coefficients are positive and $(\sigma+b+1)b(\sigma+r)>2\sigma b(r-1)$, so the cubic [Routh-Hurwitz criterion](../../../../../routh-hurwitz-stability-criterion.md) makes both new [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md) stable. Together with the [symmetry](../../../../../symmetry-physics.md) $(x,y,z)\mapsto(-x,-y,z)$ and the square-root branches, this yields the supercritical pitchfork. A local centre-manifold coordinate proportional to $x$ has leading [normal form](../../../../../normal-form-dynamical-systems.md) $\dot q=\frac\sigma{\sigma+1}(r-1)q-\frac\sigma{b(\sigma+1)}q^3+\cdots$, explicitly displaying the nonzero stabilizing cubic coefficient. At $r=1$ that cubic also gives weak local nonlinear attraction along the centre direction.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
