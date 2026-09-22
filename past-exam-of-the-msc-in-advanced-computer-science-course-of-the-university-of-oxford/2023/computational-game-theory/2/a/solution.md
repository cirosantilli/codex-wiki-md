<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Read the lower-left entry of each cell as player 1's [payoff](../../../../../payoff.md) and the upper-right entry as player 2's [payoff](../../../../../payoff.md), as indicated by the source diagram. Against $L$, player 1 strictly prefers $B$ because $2\pi>1$; against $R$, player 1 strictly prefers $T$ because $3>2$. Against $T$, player 2 strictly prefers $R$ because $6>0$; against $B$, player 2 strictly prefers $L$ because $2\sqrt2>2$. Thus the [pure strategy](../../../../../pure-strategy.md) [Nash equilibria](../../../../../nash-equilibrium.md) are

$$
\boxed{(T,R)\quad\text{and}\quad(B,L).}
$$

For a fully [mixed strategy](../../../../../mixed-strategy.md) [Nash equilibrium](../../../../../nash-equilibrium.md), write $p=\Pr(T)$ and $q=\Pr(L)$. Player 1's [expected payoffs](../../../../../expected-payoff.md) from the two [pure strategies](../../../../../pure-strategy.md) are

$$
U_1(T,q)=3-2q,\qquad
U_1(B,q)=2+(2\pi-2)q.
$$

Equality, required when both [pure strategies](../../../../../pure-strategy.md) have positive [probability](../../../../../probability.md), gives

$$
q^*=\frac1{2\pi}.
$$

Player 2's corresponding [expected payoffs](../../../../../expected-payoff.md) are

$$
U_2(p,L)=2\sqrt2(1-p),\qquad
U_2(p,R)=2+4p,
$$

so equality gives

$$
p^*=\frac{\sqrt2-1}{\sqrt2+2}=\frac{3\sqrt2-4}{2}.
$$

Both probabilities lie strictly between zero and one. Hence the unique fully [mixed strategy](../../../../../mixed-strategy.md) [Nash equilibrium](../../../../../nash-equilibrium.md) is

$$
\boxed{
\sigma_1(T)=\frac{\sqrt2-1}{\sqrt2+2},\qquad
\sigma_2(L)=\frac1{2\pi},
}
$$

with complementary probabilities on $B$ and $R$. Its [expected payoffs](../../../../../expected-payoff.md) are

$$
U_1=3-\frac1\pi,\qquad U_2=6\sqrt2-6.
$$

These are **all three [Nash equilibria](../../../../../nash-equilibrium.md)**. There are no equilibria with just one player genuinely mixing: against each opposing [pure strategy](../../../../../pure-strategy.md), the other player's [best response](../../../../../best-response.md) is unique, so that player cannot mix. When both players mix, the two linear indifference equations have the unique solution just obtained. This is [support enumeration for a bimatrix game](../../../../../support-enumeration-for-a-bimatrix-game.md) with all possible supports checked.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2023](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
