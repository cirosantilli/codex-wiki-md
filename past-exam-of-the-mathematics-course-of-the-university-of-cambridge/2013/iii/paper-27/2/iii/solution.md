<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For parameter four, the [SLE4 angle martingale](../../../../../../sle4-angle-martingale.md) is bounded, so the [Continuous-time martingale convergence theorem](../../../../../../continuous-time-martingale-convergence-theorem.md) gives an almost sure limit. The imaginary part of the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) gives

$$
\frac{d}{dt}Y_t=-\frac{2Y_t}{X_t^2+Y_t^2},
\qquad
\frac{d}{dt}Y_t^2=-4\sin^2h_t.
$$

For a point off the full simple [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) the flow exists at every finite time. If the limiting angle lay strictly between $0$ and $\pi$, the last derivative would eventually be bounded above by a strictly negative constant. That would make $Y_t^2$ negative, a contradiction. Hence **the terminal angle is either zero or $\pi$**.

The simple transient chordal [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) from $0$ to infinity splits the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) into a left component $D^-$, adjacent to the negative real boundary, and a right component $D^+$, adjacent to the positive real boundary. The [Dirichlet boundary values of the SLE angle process](../../../../../../dirichlet-boundary-values-of-the-sle-angle-process.md) identify which terminal value occurs. Indeed, run an independent [planar Brownian motion](../../../../../../planar-brownian-motion.md) from $z$ until it first hits the full [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) or the real axis. This time is finite. The Brownian path up to that time is bounded, and [Transience of chordal SLE](../../../../../../transience-of-chordal-sle.md) ensures that any [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) point it meets belongs to a finite initial segment. Thus its exit side for the truncated domains eventually agrees with its exit side for the full component. In $D^-$ every such exit is through the left bank or negative real boundary; in $D^+$ every exit is through the right bank or positive real boundary. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) in the harmonic-measure representation therefore gives

$$
\boxed{F(z)=
\begin{cases}
\pi,&z\in D^-,\\
0,&z\in D^+.
\end{cases}}
$$

This is a random side indicator, not the deterministic value $\arg z$. Uniform integrability also gives $\mathbb E[F(z)]=\arg z$, so the [SLE4 left-passage probability](../../../../../../sle4-left-passage-probability.md) is

$$
\boxed{\mathbb P(z\in D^-)=\frac{\arg z}{\pi}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
