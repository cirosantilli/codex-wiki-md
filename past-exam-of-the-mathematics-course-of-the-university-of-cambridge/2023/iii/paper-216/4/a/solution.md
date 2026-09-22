<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hamiltonian Monte Carlo](../../../../../../hamiltonian-monte-carlo.md) augments the position $x$ by an independent momentum $p\sim N(0,M)$ and uses the [Hamiltonian function](../../../../../../hamiltonian-function.md)

$$
H(x,p)=-\log\pi(x)+\frac12p^TM^{-1}p.
$$

From the current $x$, draw a fresh $p$, apply a fixed number of [leapfrog steps](../../../../../../leapfrog-integration.md) to approximate [Hamiltonian flow](../../../../../../hamiltonian-flow.md), and obtain $(x',p')$. The [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md) is

$$
1\wedge\exp\{H(x,p)-H(x',p')\};
$$

otherwise retain $x$. Momentum negation may be included to make the proposal explicitly reversible. The leapfrog map is volume preserving and reversible, while the acceptance step corrects its discretization error, leaving $\pi$ invariant after the momentum is discarded.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
