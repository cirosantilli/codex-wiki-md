<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret $x$ and $y$ as nonnegative firing-rate activities, rather than individual [action potentials](../../../../../../action-potential.md). Take $\tau,m,\sigma>0$. The relaxation time $\tau$ controls how quickly activity changes. The decay terms $-x$ and $-y$ make activity fall in the absence of recurrent drive. Each neuron receives a weighted input from the other, with coupling $a$, and the static input-output function converts that input into a target activity.

The nonlinear response tends to $m$ at large input magnitude and equals $m/2$ at $|p|=\sigma$, so $m$ is its maximum activity and $\sigma$ its half-saturation input scale. At small inputs it is approximately $mp^2/\sigma^2$. For $a>0$ this is a [mutually excitatory saturating rate network](../../../../../../mutually-excitatory-saturating-rate-network.md): increasing one neuron's activity increases the other's drive, permitting positive feedback. The response is even in $p$, so this particular equation does not model a negative $a$ as ordinary inhibition; its dynamics depend on $a^2$.

The equations combine passive relaxation with instantaneous nonlinear recurrent drive. They omit explicit spike timing, delays, channel dynamics and stochasticity, so they are an activity-level model for [computational neuroscience](../../../../../../computational-neuroscience.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
