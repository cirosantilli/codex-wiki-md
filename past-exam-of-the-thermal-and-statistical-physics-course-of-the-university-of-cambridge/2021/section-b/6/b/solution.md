<h1 id="section-b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The one-step [master equation](../../../../../master-equation.md) for the [biased random walk](../../../../../biased-random-walk.md) is

$$
P(x,t+\tau)=w_+P(x-a,t)+w_-P(x+a,t),\qquad t=N\tau.
$$

Expand in a [Taylor series](../../../../../taylor-series.md) and retain the first [time](../../../../../time-in-physics.md) [derivative](../../../../../derivative.md) and the first two space [derivatives](../../../../../derivative.md). Since $w_++w_-=1$ and $w_--w_+=2\epsilon$,

$$
\tau\partial_tP=2a\epsilon\,\partial_xP+\frac{a^2}{2}\partial_x^2P+\cdots.
$$

Thus the usual continuum truncation gives the requested [Fokker-Planck equation](../../../../../fokker-planck-equation.md),

$$
\partial_tP=D_0\partial_x^2P+C\partial_xP,\qquad
\boxed{D_0=\frac{a^2}{2\tau},\qquad C=\frac{2a\epsilon}{\tau}.}
$$

The [diffusion coefficient](../../../../../diffusion-coefficient.md) has units $\mathrm{length^2/time}$, while $C$ has units of [velocity](../../../../../velocity.md). The physical [drift velocity](../../../../../drift-velocity.md) is $v=-C=a(w_+-w_-)/\tau$, because the standard advection term is $-v\partial_xP$. A rightward bias therefore means $\epsilon<0$, $C<0$, and $v>0$.

The approximation must be stated carefully. The truncation is a controlled [diffusion limit of a weakly biased random walk](../../../../../diffusion-limit-of-a-weakly-biased-random-walk.md) when $a\to0$, $\tau\propto a^2$, and $\epsilon\propto a$, keeping $D_0$ and $C$ finite. It is also the spatial [diffusion](../../../../../diffusion.md) approximation for a continuous-time jump process with exponentially distributed waiting times of mean $\tau$.

If the original fixed-step-time walk has a finite bias, its exact [variance](../../../../../variance-split.md) from (a) instead gives the [diffusion coefficient](../../../../../diffusion-coefficient.md) of the Gaussian envelope about the drifting mean:

$$
\boxed{D_{\rm fixed}=\frac{a^2}{2\tau}(1-4\epsilon^2)=\frac{2a^2w_+w_-}{\tau}.}
$$

One obtains the same correction by retaining $\tfrac12\tau^2\partial_t^2P$ in the [time](../../../../../time-in-physics.md) expansion and using the leading advection equation to replace $\partial_t^2P$ by $v^2\partial_x^2P$. The result is $D_{\rm fixed}=D_0-v^2\tau/2$. In particular, a deterministic one-way walk has zero [variance](../../../../../variance-split.md), as this expression requires. Thus $D_0$ is the usual intended first-time-derivative approximation, not an exact variance-growth coefficient at arbitrary bias. The later continuum estimates use that convention, with the fixed-time alternative identified where relevant.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
