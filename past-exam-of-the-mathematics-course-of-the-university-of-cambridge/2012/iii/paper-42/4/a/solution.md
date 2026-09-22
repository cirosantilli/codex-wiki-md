<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The intended deletion theorem starts from the full action set $A=M\cup N$. Under that interpretation, each player's surviving action set remains nonempty: with only one action, no [mixed strategy](../../../../../../mixed-strategy.md) can weakly improve it and improve it strictly somewhere. Let the final reduced [bimatrix game](../../../../../../bimatrix-game.md) have a [Nash equilibrium](../../../../../../nash-equilibrium.md), which exists by [Nash's theorem](../../../../../../nash-s-theorem.md).

Restore the deleted actions in reverse order. Consider a row action $i$ when it is restored. At its deletion it had a weakly dominating [mixed strategy](../../../../../../mixed-strategy.md) $z$ in the then-current game. If $z_i>0$, remove that self-weight and renormalize: the strict-improvement clause guarantees $z_i<1$, and dividing the payoff comparison by $1-z_i$ gives a weakly dominating strategy supported on the other then-current row actions. Those other actions have already been restored in the reverse process. The chosen [Nash equilibrium](../../../../../../nash-equilibrium.md)'s column support lies in the final surviving set, so the dominance comparison applies to its column strategy $y$.

If the row player's [Nash equilibrium](../../../../../../nash-equilibrium.md) payoff in the restored game so far is $u$, every currently available pure row payoff against $y$ is at most $u$. The dominating mixture therefore has payoff at most $u$, and the restored action has payoff no greater than that mixture. It cannot improve the payoff. Column deviations are unchanged by adding a row action, since the actual [Nash equilibrium](../../../../../../nash-equilibrium.md) strategy remains fixed. The analogous argument works when restoring a column action. Induction restores the full game while preserving the final reduced [Nash equilibrium](../../../../../../nash-equilibrium.md) and its support.

Thus **iterated deletion of weakly dominated actions preserves at least one [Nash equilibrium](../../../../../../nash-equilibrium.md) supported entirely on surviving actions**. It need not preserve every [Nash equilibrium](../../../../../../nash-equilibrium.md) or give an order-independent reduced game.

The literal printed use of an arbitrary initial $A$ needs qualification. For example, take row payoffs $\left(\begin{smallmatrix}0&3\\1&0\end{smallmatrix}\right)$ and column payoffs $\left(\begin{smallmatrix}0&1\\0&1\end{smallmatrix}\right)$. On the restricted set containing both rows but only column $1$, row $1$ is strictly dominated by row $2$. Yet in the full game column $2$ is strictly dominant and its unique [Nash equilibrium](../../../../../../nash-equilibrium.md) uses row $1$. Deleting row $1$ based only on that restricted $A$ leaves no full-game [Nash equilibrium](../../../../../../nash-equilibrium.md) with the requested support. The proven [equilibrium preservation under iterated weak dominance](../../../../../../equilibrium-preservation-under-iterated-weak-dominance.md) therefore requires **initial $A=M\cup N$**, or concludes only about the initially restricted game.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
