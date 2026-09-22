<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In a two-player [symmetric finite game](../../../../../symmetric-finite-game.md), represent [mixed strategies](../../../../../mixed-strategy.md) by [probability](../../../../../probability.md) [vectors](../../../../../vector.md) and let $e(x,y)=x^TAy$ be the [payoff](../../../../../payoff.md) to a player using $x$ against one using $y$. A resident strategy $x^*$ is an [evolutionarily stable strategy](../../../../../evolutionarily-stable-strategy.md) if every distinct mutant strategy $y$ has an invasion barrier $\varepsilon_0(y)>0$ such that, for $0<\varepsilon<\varepsilon_0(y)$,

$$
e\bigl(x^*,(1-\varepsilon)x^*+\varepsilon y\bigr)>e\bigl(y,(1-\varepsilon)x^*+\varepsilon y\bigr).
$$

Thus when mutants are sufficiently rare, the resident has strictly larger fitness against the population mixture. The barrier may depend on the mutant; a common barrier is not part of this definition.

For fixed $y\ne x^*$ put

$$
a_y=e(x^*,x^*)-e(y,x^*),\qquad b_y=e(x^*,y)-e(y,y).
$$

By [bilinearity](../../../../../bilinearity.md) the resident-minus-mutant fitness difference is

$$
(1-\varepsilon)a_y+\varepsilon b_y.
$$

If this is positive for all sufficiently small positive $\varepsilon$, taking $\varepsilon\downarrow0$ gives $a_y\geq0$. If $a_y=0$, strict positivity requires $b_y>0$. Conversely, if $a_y>0$, choose $0<\varepsilon_0\leq a_y/[2(a_y+|b_y|)]$; then the difference is at least $a_y-\varepsilon(a_y+|b_y|)>a_y/2>0$. If $a_y=0$ and $b_y>0$, it is $\varepsilon b_y>0$ for every $0<\varepsilon<1$. This proves the [two-condition criterion for evolutionary stability](../../../../../two-condition-criterion-for-evolutionary-stability.md): **for every $y\ne x^*$, either**

$$
\boxed{e(x^*,x^*)>e(y,x^*)}
$$

**or**

$$
\boxed{e(x^*,x^*)=e(y,x^*)\quad\text{and}\quad e(x^*,y)>e(y,y).}
$$

The weak first comparison is the symmetric [Nash equilibrium](../../../../../nash-equilibrium.md) condition; the second excludes neutrally competitive mutants when that comparison is an equality.

For the [Hawk-Dove game](../../../../../hawk-dove-game.md), let $x^*=(1/2,1/2)$ and $y=(p,1-p)$, $0\leq p\leq1$. Against the resident, both [pure strategies](../../../../../pure-strategy.md) give $1/2$, so

$$
e(x^*,x^*)=e(y,x^*)=\frac12.
$$

Direct multiplication of the [payoff matrix](../../../../../payoff-matrix.md) gives

$$
e(x^*,y)=\frac32-2p,\qquad e(y,y)=1-2p^2.
$$

Consequently

$$
e(x^*,y)-e(y,y)=2\left(p-\frac12\right)^2>0\qquad(p\ne1/2).
$$

The equality case of the [two-condition criterion for evolutionary stability](../../../../../two-condition-criterion-for-evolutionary-stability.md) therefore applies to every distinct mutant. More explicitly, the fitness difference in a mixed population is $2\varepsilon(p-1/2)^2$, positive for every $0<\varepsilon<1$. Hence **$\boxed{(1/2,1/2)\text{ is an evolutionarily stable strategy}}$**, with the common invasion barrier one.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
