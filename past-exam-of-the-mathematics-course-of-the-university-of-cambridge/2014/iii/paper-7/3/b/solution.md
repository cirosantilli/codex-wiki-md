<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Fubini's theorem](../../../../../../fubini-s-theorem.md) and [integral](../../../../../../integral.md) [triangle inequality](../../../../../../triangle-inequality.md) give

$$
 \boxed{\|\rho(g)\|_{L^1_x}\leq\int\int|g(x,v)|\,dv\,dx=\|g\|_1.}
$$

Define the [normalized velocity-reset collision operator](../../../../../../normalized-velocity-reset-collision-operator.md) using the [normalized velocity-reset projection](../../../../../../normalized-velocity-reset-projection.md) $Pg(x,v)=\rho(g)(x)M(v)$ and $B=P-I$. Since $M\geq0$ and $\int M=1$,

$$
 \|Pg\|_1=\|\rho(g)\|_{L^1_x}\leq\|g\|_1,
 \qquad \|Bg\|_1\leq2\|g\|_1.
$$

Also $P^2=P$; the collision gain replaces the velocity distribution by $M$ while preserving the spatial mass. In [Bochner integral](../../../../../../bochner-integral.md) notation the printed, undamped source operator is

$$
 (\tau f)(t)=\int_0^tU_{t-s}Bf(s)\,ds.
$$

Using the transport [isometry](../../../../../../isometry.md) and the [integral](../../../../../../integral.md) [triangle inequality](../../../../../../triangle-inequality.md) proves

$$
 \boxed{\|\tau f(t)\|_1\leq2\int_0^t\|f(s)\|_1\,ds
 \leq2t\sup_{0\leq s\leq t}\|f(s)\|_1.}
$$

These estimates hold for measurable, locally time-bounded $E$-valued functions. If the displayed supremum is infinite, the numerical bound is interpreted in the extended sense; the construction below works in a space where it is finite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
