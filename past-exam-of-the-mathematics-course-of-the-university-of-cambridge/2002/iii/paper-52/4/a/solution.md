<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $W\geq0$ be the downward fluid suction speed and $V\geq0$ the downward particle [settling velocity](../../../../../../settling-velocity.md) relative to that fluid. Set $Q=uh$ and $g'=g'_0\phi$. The carrier [volume conservation](../../../../../../volume-conservation.md) and particle-volume balances per unit channel width are

$$
\boxed{Q'=-W,\qquad (Q\phi)'=-(W+V)\phi.}
$$

The particle sink includes suction as well as relative settling: the particles follow the well-mixed withdrawn fluid, in addition to settling through it. Subtracting $\phi Q'$ yields $Q\phi'=-V\phi$. Thus for $W>0$, as long as $Q>0$,

$$
\boxed{Q=Q_0-Wx,\qquad\phi=\left(1-\frac{Wx}{Q_0}\right)^{V/W}.}
$$

For $W=0$ the continuous limit is $Q=Q_0$ and $\phi=e^{-Vx/Q_0}$. In particular suction alone does not change the well-mixed particle fraction: $V=0$ implies $\phi=1$.

Withdrawn fluid carries its local horizontal [momentum](../../../../../../momentum.md), so the [momentum flux](../../../../../../momentum-flux.md) and [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) force obey

$$
\boxed{\left(hu^2+\frac12g'_0\phi h^2\right)'=-Wu.}
$$

Expand this and use $Q'=-W$. The suction [momentum](../../../../../../momentum.md) terms cancel in the primitive acceleration equation, leaving

$$
uu'+g'_0\phi h'+\frac12g'_0h\phi'=0.
$$

These are the governing equations for a [particle-laden current with suction](../../../../../../particle-laden-current-with-suction.md). Substituting $u=Q/h$ and the [concentration](../../../../../../concentration.md) equation gives the convenient depth equation

$$
\boxed{(1-\operatorname{Fr}^2)h'=\frac{Wu}{g'_0\phi}+\frac{Vh}{2Q},\qquad \operatorname{Fr}^2=\frac{u^2}{g'_0\phi h}.}
$$

The steady carrier flux is exhausted at the formal length $\boxed{x_*=Q_0/W}$ when $W>0$. Positive $Q$ cannot continue beyond it. Near that limit a chosen depth branch, mixing or shallow-layer assumptions may fail, so this is the mass-budget extent, not a guarantee that every arbitrary inlet state has a regular shallow continuation to it. When $W=0$, settling makes the driving [reduced gravity](../../../../../../reduced-gravity-split.md) exponentially small but does not remove carrier fluid; this ideal steady model has no finite mass-budget runout.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Section B](../../section-b.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
