<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X,Y$ be two solutions with the same Brownian driver and the same initial value. Write $D=X-Y$, and take a common [Lipschitz](../../../../../../lipschitz-continuity.md) constant $L$ for both coefficients. Stop when $|X|+|Y|$ reaches $n$. Before this [stopping time](../../../../../../stopping-time.md) $\tau_n$, all difference integrands below are bounded. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d(D^2)=2D[\sigma(X)-\sigma(Y)]\,dB
+\left([\sigma(X)-\sigma(Y)]^2+2D[b(X)-b(Y)]\right)dt.
$$

The stopped [stochastic integral](../../../../../../stochastic-integral.md) is a true [martingale](../../../../../../martingale-split.md) on every finite horizon. [Lipschitz continuity](../../../../../../lipschitz-continuity.md) therefore yields

$$
\mathbb E D_{t\wedge\tau_n}^2
\le(L^2+2L)\int_0^t\mathbb E[\mathbf1_{\{s<\tau_n\}}D_s^2]ds
\le(L^2+2L)\int_0^t\mathbb E D_{s\wedge\tau_n}^2ds.
$$

Since $D_0=0$, the [Gronwall inequality](../../../../../../gronwall-inequality.md) makes the left side zero. Let $n\to\infty$; the continuous global solutions are bounded on each compact time interval, so their [stopping times](../../../../../../stopping-time.md) exhaust it. Equality first at every rational time and then by continuity gives indistinguishability. This proves **[pathwise uniqueness](../../../../../../pathwise-uniqueness.md) for globally [Lipschitz](../../../../../../lipschitz-continuity.md) drift and diffusion coefficients**. The argument does not require the initial value to have a global second moment: after stopping, the difference is bounded and initially zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
