<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $g_t=P_{1-t}(\nabla f)(X_t)$. The [triangle inequality](../../../../../../triangle-inequality.md) for the conditional average gives

$$
\lVert g_t\rVert\le P_{1-t}(\lVert\nabla f\rVert)(X_t)\le K.
$$

The independent coordinate [Brownian motions](../../../../../../brownian-motion-split.md) have zero cross-variation, so the [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) gives

$$
\boxed{[M]_1=\int_0^1\lVert g_t\rVert^2\,dt\le K^2.}
$$

The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) says that a [continuous local martingale](../../../../../../continuous-local-martingale.md) $N$ starting at zero whose [quadratic variation](../../../../../../quadratic-variation.md) diverges admits a [Brownian motion](../../../../../../brownian-motion-split.md) $B$, with the inverse-clock filtration, such that $N_t=B_{[N]_t}$. If the total clock is finite, one may enlarge the probability space and append independent [Brownian motion](../../../../../../brownian-motion-split.md) after the clock terminates. This gives the same identity up to the original lifetime.

Apply this theorem to $N=M-M_0$. The clock bound implies the event inclusion

$$
\{|M_1-M_0|>r\}\subseteq\left\{\sup_{0\le s\le K^2}|B_s|>r\right\}.
$$

The latter event is contained in the union of the upper and lower crossing events. Symmetry of [Brownian motion](../../../../../../brownian-motion-split.md) gives

$$
\boxed{\mathbb P(|M_1-M_0|>r)\le2\mathbb P\left(\sup_{0\le s\le K^2}B_s>r\right).}
$$

This uses only an event inclusion; independence between the [Brownian motion](../../../../../../brownian-motion-split.md) and its random clock is neither assumed nor needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
