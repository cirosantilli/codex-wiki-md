<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

[Nash's theorem](../../../../../nash-s-theorem.md) says that every finite game, including a two-player game with two pure choices each, has at least one [Nash equilibrium](../../../../../nash-equilibrium.md) in [mixed strategies](../../../../../mixed-strategy.md).

For player $1$, holding $p_2$ fixed, the [expected value](../../../../../expected-value.md) of the payoff is

$$
E_1=-Up_1p_2+2p_1(1-p_2)-2(1-p_1)p_2+(1-p_1)(1-p_2)
=1-3p_2+p_1\bigl[1-(U-1)p_2\bigr].
$$

It is an [affine function](../../../../../affine-function.md) of $p_1$. Therefore player $1$ chooses $p_1=1$ when $1-(U-1)p_2>0$, chooses $p_1=0$ when it is negative, and is indifferent when it vanishes. By [symmetry](../../../../../symmetry-physics.md), player $2$ has the analogous [best response](../../../../../best-response.md).

If $U<2$, then $1-(U-1)p>0$ for every $p\in[0,1]$, so becoming a Dark Lord with probability one is a [strictly dominant strategy](../../../../../strictly-dominant-strategy.md). The unique equilibrium is

$$
\boxed{(p_1,p_2)=(1,1).}
$$

If $U>2$, each player is indifferent when the other chooses $p=1/(U-1)$. This gives one interior mixed equilibrium, while the two asymmetric pure equilibria arise because a player facing a certain peasant chooses Lord and a player facing a certain Lord chooses peasant. The three equilibria are

$$
\boxed{(1,0),\qquad(0,1),\qquad
\left(\frac1{U-1},\frac1{U-1}\right).}
$$

Consequently $\boxed{U_0=2}$. At the threshold itself there is a continuum of equilibria with $p_1=1$ or $p_2=1$, consistent with the question's strict inequalities.

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
