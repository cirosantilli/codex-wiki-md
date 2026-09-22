<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

One analysis can treat a reported symptom-onset date as the exact $H\to I$ transition time. That adds an exactly observed infection-time density to the likelihood, but assumes symptoms begin immediately at infection, every relevant episode is symptomatic, and dates are recalled and reported without error.

A more realistic analysis treats true infection as a latent transition and symptom onset as a noisy observation. A reporting-delay distribution, and possibly probabilities of asymptomatic infection and non-reporting, can be added to a [Hidden Markov model](../../../../../../hidden-markov-model.md). Weekly tests then interval-censor the state transition while the symptom date refines its distribution. This approach uses more information but requires an identifiable and correctly specified symptom-delay and reporting model.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
