<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work with the [filtration](../../../../../filtration-probability-theory.md) relative to which the given [Brownian motion](../../../../../brownian-motion-split.md) or [Markov jump process](../../../../../markov-jump-process.md) has its stated properties. All [martingale](../../../../../martingale-split.md) assertions below concern every finite time interval; no infinite-horizon [uniform integrability](../../../../../uniform-integrability.md) is claimed.

First put $C=\sup_x|\sigma(x)|$. The solution has the representation $X_t=\int_0^t\sigma(X_s)dB_s$, and the [Itô isometry](../../../../../ito-isometry.md) gives

$$
\mathbb EX_t^2=\mathbb E\int_0^t\sigma(X_s)^2ds\le C^2t.
$$

Thus $X$ is a square-integrable [martingale](../../../../../martingale-split.md), not just a [local martingale](../../../../../local-martingale.md). Applying the [Itô formula](../../../../../ito-s-lemma.md) to its square cancels the finite-variation term and gives

$$
Z_t=2\int_0^tX_s\sigma(X_s)dB_s.
$$

The expected squared integrand integral is bounded by

$$
4\mathbb E\int_0^tX_s^2\sigma(X_s)^2ds\le4C^2\int_0^tC^2s\,ds=2C^4t^2.
$$

Therefore **both $X$ and $Z$ are true square-integrable [martingales](../../../../../martingale-split.md)**. This is the [bounded diffusion coefficient gives square martingales](../../../../../bounded-diffusion-coefficient-gives-square-martingales.md) criterion. Only bounded measurability of the coefficient and existence of the stipulated solution have been used.

For the jump process, the [Lévy kernel of a Markov jump process](../../../../../levy-kernel-of-a-markov-jump-process.md) uses displacements: a mark $y$ sends the state $x$ to $x+y$. Let $\Lambda=\sup_x\lambda(x)$ and $V=\sup_xv(x)$. The bounded total rate prevents explosion; the number of jumps on a finite interval is dominated by a rate-$\Lambda$ [Poisson process](../../../../../poisson-process.md). Let $N(ds,dy)$ record the jump displacements. Its [predictable compensator of a jump measure](../../../../../predictable-compensator-of-a-jump-measure.md) is

$$
\nu(ds,dy)=K(X_{s-},dy)ds.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\int |y|K(x,dy)\le\sqrt{\lambda(x)v(x)}$, so the zero first moment is absolutely meaningful. Since that moment vanishes,

$$
X_t=\int_0^t\int_{\mathbb R}y\,(N-\nu)(ds,dy),\qquad \mathbb EX_t^2=\mathbb E\int_0^tv(X_{s-})ds\le Vt.
$$

The compensated integral is a square-integrable [martingale](../../../../../martingale-split.md): its isometry follows first for bounded marks from conditional compensation and then by truncation in the squared-integrand [norm](../../../../../norm.md).

The jump version of the square [Itô formula](../../../../../ito-s-lemma.md) is $X_t^2=2\int_0^tX_{s-}dX_s+\sum_{s\le t}(\Delta X_s)^2$. Hence

$$
Z_t=2\int_0^tX_{s-}dX_s+\int_0^t\int_{\mathbb R}y^2(N-\nu)(ds,dy).
$$

The first term is square [integrable](../../../../../integrability.md) because

$$
4\mathbb E\int_0^tX_{s-}^2v(X_{s-})ds\le2V^2t^2.
$$

The second is an [integrable](../../../../../integrability.md) [martingale](../../../../../martingale-split.md): the expected absolute uncompensated jump-square sum is at most $Vt$, and the compensator identity, multiplied by any bounded event known at an earlier time, makes its increments conditionally centered. Values $X_s$ and $X_{s-}$ agree for Lebesgue-almost every time, so the displayed compensation is exactly the one defining $Z$. Thus **$X$ and $Z$ are true [martingales](../../../../../martingale-split.md) in the jump case as well**. A fourth moment of the jumps is unnecessary; in particular we have not asserted that this $Z$ must be square [integrable](../../../../../integrability.md). This is [centered finite-rate jump kernel gives square martingales](../../../../../centered-finite-rate-jump-kernel-gives-square-martingales.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
