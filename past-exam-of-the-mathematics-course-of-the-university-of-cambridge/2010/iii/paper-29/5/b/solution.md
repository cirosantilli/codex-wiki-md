<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [quadratic covariation](../../../../../../quadratic-covariation.md) of two [continuous semimartingales](../../../../../../continuous-semimartingale.md) by polarization:

$$
[X,Y]_t=\frac14\bigl([X+Y]_t-[X-Y]_t\bigr).
$$

The available [quadratic variation](../../../../../../quadratic-variation.md) convergence theorem and the [polarization identity](../../../../../../polarization-identity.md) imply that the sums of products of simultaneous grid increments converge in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md) to $[X,Y]$. The [quadratic covariation](../../../../../../quadratic-covariation.md) is a continuous finite-variation process, vanishing at time zero.

For a grid ending at $t_n=h_n\lfloor t/h_n\rfloor$, the elementary algebraic identity

$$
X_{(k+1)h_n}Y_{(k+1)h_n}-X_{kh_n}Y_{kh_n}
=X_{kh_n}\Delta_kY+Y_{kh_n}\Delta_kX+\Delta_kX\Delta_kY
$$

telescopes. The first two sums converge by part (a), with the continuous processes $X,Y$ as integrands; continuous paths are left-continuous and locally bounded. The last sum converges to the [quadratic covariation](../../../../../../quadratic-covariation.md) by the preceding polarization argument. Finally, $X_{t_n}Y_{t_n}\to X_tY_t$ locally uniformly by continuity. Hence

$$
\boxed{X_tY_t=X_0Y_0+\int_0^tX_s\,dY_s+\int_0^tY_s\,dX_s+[X,Y]_t.}
$$

This is the [Itô product rule](../../../../../../ito-product-rule.md), or stochastic [integration by parts](../../../../../../integration-by-parts.md). Uniqueness of the limit in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md), followed by continuity, makes the identity hold simultaneously for all $t$ outside one null set. The proof used finite-grid algebra, part (a), and the permitted [quadratic variation](../../../../../../quadratic-variation.md) theorem; it did not use the [Itô formula](../../../../../../ito-s-lemma.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
