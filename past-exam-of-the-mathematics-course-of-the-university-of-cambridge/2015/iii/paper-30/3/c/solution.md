<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The scalar [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) states that an [adapted process](../../../../../../adapted-process.md) $X$ starting at zero is a [Brownian motion](../../../../../../brownian-motion-split.md) if and only if it is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with

$$
\boxed{\langle X\rangle_t=t.}
$$

For necessity, the centered independent increments make a [Brownian motion](../../../../../../brownian-motion-split.md) a [martingale](../../../../../../martingale-split.md). Their conditional second moments show that $X_t^2-t$ is also a [martingale](../../../../../../martingale-split.md). The defining uniqueness of the [quadratic variation](../../../../../../quadratic-variation.md) compensator gives $\langle X\rangle_t=t$.

For sufficiency, fix $\theta\in\mathbb R$ and apply the [Itô formula](../../../../../../ito-s-lemma.md) to

$$
Z_t=\exp\left(i\theta X_t+\frac{\theta^2t}{2}\right).
$$

The time drift cancels the second-order Itô term, leaving $dZ_t=i\theta Z_t\,dX_t$. Its real and imaginary parts are [local martingales](../../../../../../local-martingale.md). On any deterministic interval $[0,T]$, $|Z_t|=e^{\theta^2t/2}\leq e^{\theta^2T/2}$, so the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md) makes them true [martingales](../../../../../../martingale-split.md). Therefore

$$
\mathbb E[e^{i\theta(X_t-X_s)}\mid\mathcal F_s]
=e^{-\theta^2(t-s)/2}.
$$

Part (b) proves the Brownian property. This also supplies a proof of [Lévy's characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) through conditional Fourier transforms.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
