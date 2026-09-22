<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $p=\mathbb P(y_\tau=\alpha)$. For $k\ne2$, the bounded stopped martingale from part (b) converges to $y_\tau^{2-k}$, so the [dominated convergence theorem](../../../../dominated-convergence-theorem.md) gives

$$
1=p\alpha^{2-k}+(1-p)\beta^{2-k}.
$$

Therefore the [boundary hitting probability from a diffusion scale function](../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md) is

$$
\boxed{p=\frac{1-\beta^{2-k}}{\alpha^{2-k}-\beta^{2-k}}\quad(k\ne2).}
$$

For $k=2$, applying [Itô's formula](../../../../ito-s-lemma.md) to $\log Y_t$ gives a bounded stopped martingale instead, yielding

$$
\boxed{p=\frac{\log\beta}{\log\beta-\log\alpha}\quad(k=2).}
$$

If $k>2$ and $\beta>1$ is fixed, the first expression tends to zero as $\alpha\downarrow0$. A continuous path that reaches zero before it reaches $\beta$ must first reach every such $\alpha$ before $\beta$, so that event has probability zero. Any path hitting zero in finite time has a finite maximum up to that time, and therefore belongs to one of these zero-probability events with an integer upper boundary $\beta>1$. Their countable union still has probability zero. Thus **the process does not hit zero almost surely**. This is the relevant part of the [Hitting-zero classification for a Bessel process](../../../../hitting-zero-classification-for-a-bessel-process.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
