<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Decompose the required runway into successive layers. The first layer has cost $s$ and is needed by all four planes. The next costs $2s$ and is needed by the three medium-or-long planes. The final layer costs $4s$ and is needed only by the longest plane.

For each layer, the first requiring plane in a uniformly random ordering contributes its entire cost. Each of its requiring planes has equal probability of being first. By [linearity of the Shapley value](../../../../../linearity-of-the-shapley-value.md), divide each layer cost equally among those requiring it. The payments are therefore

$$
\boxed{\phi_{\mathrm{short}}=\frac s4,\qquad\phi_{\mathrm{medium},1}=\phi_{\mathrm{medium},2}=\frac s4+\frac{2s}3=\frac{11s}{12},\qquad\phi_{\mathrm{long}}=\frac s4+\frac{2s}3+4s=\frac{59s}{12}.}
$$

They sum to $7s=c(N)$. The equality of the two medium payments follows from their identical runway requirements; the random-order argument proves the amounts, not just their equality.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
