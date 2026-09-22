<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the same affine drift cancellation with terminal conditions $a(0)=0$, $b(0)=1$. It gives $a(\tau)=0$, $b(\tau)=e^{-\tau}$, so

$$
D_te^{-(T-t)}r_t
=\mathbb E^{\mathbb Q}[D_Tr_T\mid\mathcal F_t].
$$

The process is bounded, which justifies the [conditional expectation](../../../../../../conditional-expectation.md) identity. The [Bayes formula for conditional expectation](../../../../../../bayes-formula-for-conditional-expectation.md) for the [forward measure](../../../../../../forward-measure.md) now gives

$$
\begin{aligned}
\mathbb E^{\mathbb Q_T}[r_T\mid\mathcal F_t]
&=\frac{\mathbb E^{\mathbb Q}[D_Tr_T\mid\mathcal F_t]}
{\mathbb E^{\mathbb Q}[D_T\mid\mathcal F_t]}\\
&=\boxed{\frac{e^{-(T-t)}r_t}{1-(1-e^{-(T-t)})r_t}}.
\end{aligned}
$$

The denominator is positive; the ratio lies in $[0,1]$ and equals $r_T$ at maturity. This is the [forward-measure terminal rate in a linear bond model](../../../../../../forward-measure-terminal-rate-in-a-linear-bond-model.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
