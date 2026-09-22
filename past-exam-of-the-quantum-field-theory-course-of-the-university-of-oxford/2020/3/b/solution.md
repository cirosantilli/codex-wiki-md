<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the interacting [vacuum state](../../../../vacuum-state.md) defined perturbatively by the same [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md), the normalized [time-ordered product](../../../../time-ordered-product.md) is

$$
\boxed{\left\langle T\prod_{r=1}^m\phi(x_r)\right\rangle
=\left.\frac{1}{Z[\lambda;0]}\frac1{i^m}
\frac{\delta^m Z[\lambda;j]}{\delta j(x_1)\cdots\delta j(x_m)}\right|_{j=0}.}
$$

Each [functional derivative](../../../../functional-derivative.md) inserts $i\phi$, accounting for $i^{-m}$. The denominator implements [cancellation of vacuum bubbles](../../../../cancellation-of-vacuum-bubbles.md), while disconnected pieces carrying external insertions still contribute. The lower limit $i=i$ in the printed product is a typographical error; the product here runs from 1 to $m$.

At order $V$ in the cubic scalar [field interaction term](../../../../field-interaction-term.md), the expansion of the [generating functional](../../../../generating-functional.md) supplies $1/[V!(3!)^V]$. The $V!$ counts permutations of indistinguishable integrated [interaction vertices](../../../../interaction-vertex.md), and $3!$ counts permutations of the three field slots at each [interaction vertex](../../../../interaction-vertex.md). Applying the [Wick theorem](../../../../wick-s-theorem.md) pairs fields into [Feynman propagators](../../../../feynman-propagator.md). Several pairings produce the same [Feynman diagram](../../../../feynman-diagram.md); their number $N_G$ multiplies the expansion coefficient. For fixed labelled external points, the net combinatorial weight is

$$
\boxed{w_G=\frac{N_G}{V!(3!)^V}=\frac1{S_G}.}
$$

Here $S_G$ is the order of the graph's [automorphism group](../../../../automorphism-group.md) when the external labels are fixed, with permutations of identical parallel lines and reversal of a self-loop included as applicable. This is the [Feynman-diagram symmetry factor](../../../../feynman-diagram-symmetry-factor.md) convention in which a [Feynman diagram](../../../../feynman-diagram.md) is divided by $S_G$. Each cubic [interaction vertex](../../../../interaction-vertex.md) then contributes $-i\lambda$, each line contributes $\Delta_F$, and each internal vertex is integrated over its position. External labelled points are not divided by $m!$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
