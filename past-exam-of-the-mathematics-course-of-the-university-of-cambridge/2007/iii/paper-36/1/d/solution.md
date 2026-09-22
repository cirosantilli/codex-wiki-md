<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Brownian scaling](../../../../../../brownian-scaling.md) gives $|B_t|\overset{d}=\sqrt t\,R$, where $R=|B_1|$ has [Rayleigh distribution](../../../../../../rayleigh-distribution.md) with density $r e^{-r^2/2}$, $r>0$. For every $p>0$,

$$
\mathbb E|\log R|^p=\int_0^\infty|\log r|^p r e^{-r^2/2}\,dr<\infty.
$$

Near zero this is bounded by $\int_0^1|\log r|^p r\,dr=\int_0^\infty u^pe^{-2u}\,du$, which is finite; near infinity the Gaussian tail dominates any logarithmic power. The inequality $|a+b|^p\le C_p(|a|^p+|b|^p)$, valid also for $0<p<1$, now yields

$$
\boxed{\mathbb E|X_t|^p<\infty\qquad(t\ge1,\ p>0).}
$$

Let $c=\mathbb E\log R$, a finite constant. The same scaling identity gives

$$
\boxed{\mathbb E X_t=\tfrac12\log t+c\longrightarrow\infty.}
$$

An integrable [martingale](../../../../../../martingale-split.md) has constant expectation, so the [logarithm of planar Brownian radius](../../../../../../logarithm-of-planar-brownian-radius.md) is a [strict local martingale](../../../../../../strict-local-martingale.md) on $[1,\infty)$. Fixed-time integrability, even of every positive power, does not imply the stopping-time [uniform integrability](../../../../../../uniform-integrability.md) required in part a.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
