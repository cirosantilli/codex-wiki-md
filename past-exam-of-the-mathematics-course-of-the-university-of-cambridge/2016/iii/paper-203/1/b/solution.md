<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A finite original exit time alone does not imply that the integral defining the [conformal Brownian clock](../../../../../../conformal-brownian-clock.md) is finite. To establish this, let $\psi=\phi^{-1}$. On the event $\{\widetilde T=\infty\}$, the Brownian path of part (a) lives forever in $D'$, while its inverse clock satisfies

$$
\tau(t)=\int_0^t|\psi'(\widetilde B_r)|^2\,dr<T.
$$

Choose a closed disc $C$ compactly contained in $D'$. Its radius may be decreased so that $|\psi'|^2\geq c>0$ on $C$. [Recurrence of planar Brownian motion](../../../../../../recurrence-of-planar-brownian-motion.md), together with the [Strong Markov property](../../../../../../strong-markov-property.md), gives infinite total [Brownian occupation time](../../../../../../brownian-occupation-time.md) in $C$: return repeatedly to a smaller concentric disc, and use the fixed positive probability of remaining in $C$ for a fixed positive duration. The successive trials imply infinitely many such durations. This is the same mechanism as the [divergence of a positive planar Brownian occupation integral](../../../../../../divergence-of-a-positive-planar-brownian-occupation-integral.md).

Hence, on any infinite-lifetime Brownian path,

$$
\int_0^\infty|\psi'(\widetilde B_r)|^2\,dr
\geq c\int_0^\infty\mathbf1_C(\widetilde B_r)\,dr=\infty.
$$

This contradicts $\tau(t)<T<\infty$. Thus $\widetilde T$ is finite [almost surely](../../../../../../almost-sure-convergence.md), and equality in law from part (a) gives **[finite exit from a conformal image of a bounded planar domain](../../../../../../finite-exit-from-a-conformal-image-of-a-bounded-planar-domain.md)**:

$$
\boxed{\mathbb P_{z'}(T'<\infty)=1.}
$$

This asserts almost-sure finiteness, not finiteness of the expected exit time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
