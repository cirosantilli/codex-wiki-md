<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The unique [Nash equilibrium](../../../../../nash-equilibrium.md) uses row [probabilities](../../../../../probability.md) $(2/7,5/7)$ on $(T,B)$ and column [probabilities](../../../../../probability.md) $(4/7,3/7)$ on $(L,R)$. The [value of a zero-sum game](../../../../../value-of-a-zero-sum-game.md) to the row player is $-1/7$; the column player receives $1/7$.**

The first graph solves the row player's max–min [optimization](../../../../../mathematical-optimization-split.md): choose a [mixed strategy](../../../../../mixed-strategy.md) guaranteeing the greatest possible worst-case [expected payoff](../../../../../expected-payoff.md). The second solves the column player's min–max [optimization](../../../../../mathematical-optimization-split.md): choose a [mixed strategy](../../../../../mixed-strategy.md) placing the smallest upper bound on the row player's [expected payoff](../../../../../expected-payoff.md). Their optimal heights agree, illustrating the [minimax theorem](../../../../../minimax-theorem.md).

There is also a direct [Nash equilibrium](../../../../../nash-equilibrium.md) certificate, so the conclusion does not depend on reading coordinates from a plot. At $p^*=2/7$, both opposing pure columns give row [expected payoff](../../../../../expected-payoff.md) $-1/7$; at $q^*=4/7$, both pure rows give row [expected payoff](../../../../../expected-payoff.md) $-1/7$. By linearity, every [unilateral deviation](../../../../../unilateral-deviation.md), including an arbitrary [mixed strategy](../../../../../mixed-strategy.md), leaves the deviator's [expected payoff](../../../../../expected-payoff.md) unchanged against the fixed opposing equilibrium mixture. Neither player can improve it. This is a [mixed-strategy optimality certificate for a matrix game](../../../../../mixed-strategy-optimality-certificate-for-a-matrix-game.md).

The equilibrium outcome is a [probability distribution](../../../../../probability-distribution-split.md) over cells, rather than one deterministic cell. [Independent](../../../../../independent-random-variables.md) randomization gives

$$
\boxed{\Pr(TL)=\frac8{49},\quad \Pr(TR)=\frac6{49},\quad
\Pr(BL)=\frac{20}{49},\quad \Pr(BR)=\frac{15}{49}.}
$$

The resulting row [expected payoff](../../../../../expected-payoff.md) is $(16-18-20+15)/49=-1/7$. Finally, each envelope has a unique optimum, so any [Nash equilibrium](../../../../../nash-equilibrium.md) must use the displayed [optimal mixed strategies](../../../../../optimal-mixed-strategy.md). In particular there is no [pure strategy](../../../../../pure-strategy.md) [Nash equilibrium](../../../../../nash-equilibrium.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
