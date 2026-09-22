<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

For a normalized state and a [self-adjoint operator](../../../../../self-adjoint-operator.md) $Q$ with finite second moment, the [quantum uncertainty](../../../../../quantum-uncertainty.md) is defined by $\Delta Q=\|(Q-\langle Q\rangle)\psi\|$. Since $\langle Q\rangle$ is real,

$$
 (\Delta Q)^2=\langle(Q-\langle Q\rangle)^2\rangle
 =\boxed{\langle Q^2\rangle-\langle Q\rangle^2}.
$$

In an energy [eigenstate](../../../../../eigenstate.md) of the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md),

$$
 E=\langle H\rangle
 =\frac{(\Delta p)^2+\langle p\rangle^2}{2m}
 +\frac{m\omega^2}{2}\bigl((\Delta x)^2+\langle x\rangle^2\bigr).
$$

Discarding the nonnegative squared means proves the stated lower bound. The [Heisenberg uncertainty principle](../../../../../heisenberg-uncertainty-relation.md) is $\Delta x\,\Delta p\geq\hbar/2$, following from $[x,p]=i\hbar$. Applying the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) to the two variance contributions gives

$$
 E\geq\frac{(\Delta p)^2}{2m}+\frac{m\omega^2(\Delta x)^2}{2}
 \geq\omega\Delta p\Delta x\geq\boxed{\frac{\hbar\omega}{2}}.
$$

Here $\omega>0$ is the oscillator frequency. The bound is the ground-state energy; equality requires zero means and the appropriate minimum-uncertainty width.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
