<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [random-walk update](../../../../../../../random-walk-metropolis-algorithm.md) proposes $\theta'=\theta+\eta$, with an increment distribution independent of the current state. If its density is symmetric, $q(\theta'\mid\theta)=q(\theta\mid\theta')$, reducing the [Metropolis–Hastings acceptance probability](../../../../../../../metropolis-hastings-acceptance-probability.md) to $\min\{1,\pi(\theta')/\pi(\theta)\}$. For nonsymmetric increments the proposal-density ratio must remain.

Such updates need little global knowledge of the target and adapt naturally to its local scale. Their limitation is a tuning tradeoff: very small increments accept often but move slowly, while very large increments are often rejected. They can also have difficulty moving between distant modes. Covariance-scaled increments help with anisotropic targets, but the chain still explores through local steps.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
