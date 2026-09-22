<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\pi$ denote the posterior and let the proposal density satisfy $q(\theta'\mid\theta)=q(\theta\mid\theta')$. For distinct states, the Metropolis transition density is

$$
P(\theta,\theta')=q(\theta'\mid\theta)
\min\{1,\pi(\theta')/\pi(\theta)\}.
$$

Consequently

$$
\pi(\theta)P(\theta,\theta')
=q(\theta'\mid\theta)\min\{\pi(\theta),\pi(\theta')\}
=\pi(\theta')P(\theta',\theta).
$$

The rejection mass on the diagonal also satisfies [detailed balance](../../../../../../detailed-balance.md), so the posterior is invariant.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
