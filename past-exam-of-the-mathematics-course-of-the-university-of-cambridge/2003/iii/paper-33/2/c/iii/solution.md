<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $C_u=\int_0^u e^{2W_s}ds$. Its paths are continuous and strictly increasing. We also need $C_\infty=\infty$ to ensure that the printed inverse is finite for every $t$.

Here is a duration argument for [Divergence of a driftless Brownian exponential clock](../../../../../../../divergence-of-a-driftless-brownian-exponential-clock.md). Start at zero and choose successive return times $T_j$ to zero, each at least one time unit after the preceding return. [Recurrence of one-dimensional Brownian motion](../../../../../../../recurrence-of-one-dimensional-brownian-motion.md) makes all these times finite. By the [Strong Markov property](../../../../../../../strong-markov-property.md), each unit interval after $T_j$ has the same fixed positive probability that the Brownian path stays above $-1$. The intervals are disjoint, and repeated strong Markov conditioning makes these trials independent. Infinitely many succeed almost surely, by the [Borel-Cantelli lemma](../../../../../../../borel-cantelli-lemmas.md). Each successful interval contributes at least $e^{-2}$ to $C_\infty$, proving divergence.

Therefore $\tau_t$ is the unique finite inverse of $C$, with $C_{\tau_t}=t$. It is an increasing family of stopping times, since $\{\tau_t\leq u\}=\{C_u\geq t\}$. The continuous-local-martingale time-change theorem states that inverse-bracket time change preserves the local-martingale property in the filtration $\mathcal G_t=\mathcal F_{\tau_t}$ and transforms the bracket by composition. Applied to $Y$, this gives

$$
[Z]_t=[Y]_{\tau_t}=C_{\tau_t}=t,\qquad Z_0=1.
$$

The [Lévy characterization of Brownian motion](../../../../../../../levy-characterization-of-brownian-motion.md) now proves that **$Z$ is Brownian motion starting at one; $Z-1$ is standard Brownian motion**, in the time-changed filtration. If the term Brownian motion is reserved for a process starting at zero, $Z$ itself fails only that normalization. The substantive Brownian property, including independent Gaussian increments in the new time, holds.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
