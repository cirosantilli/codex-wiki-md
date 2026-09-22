# Mixed strategy

↑ **Parent:** [Game theory](game-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mixed_strategy)

A [mixed strategy](mixed-strategy.md) is a [probability distribution](probability-distribution-split.md) over a player's [pure strategies](pure-strategy.md). For a [finite game](finite-game.md) with $m_i$ such strategies, the possible [mixed strategies](mixed-strategy.md) form the [probability simplex](probability-simplex.md)

$$
\Delta(S_i)=\left\{\sigma_i\in\mathbb R^{m_i}:\sigma_i(a)\geq0,\quad\sum_{a\in S_i}\sigma_i(a)=1\right\}.
$$

A [pure strategy](pure-strategy.md) is included as a [mixed strategy](mixed-strategy.md) placing all [probability](probability.md) on one choice. The [support of a mixed strategy](support-of-a-mixed-strategy.md) consists of the choices with positive [probability](probability.md). In a sequential game, sampling a complete [pure strategy](pure-strategy.md) once is the definition; it is not automatically equivalent to fresh randomization at every move.

In a [bimatrix game](bimatrix-game.md), write $A$ for the row player's [payoff matrix](payoff-matrix.md) and $B$ for the column player's, and write $x,y$ for their [probability](probability.md) [vectors](vector.md). [Independent](independent-random-variables.md) randomization gives [expected payoffs](expected-payoff.md)

$$
U_1(x,y)=x^{\mathsf T}Ay,\qquad U_2(x,y)=x^{\mathsf T}By.
$$

For example, in [matching pennies](matching-pennies.md), choosing heads with [probabilities](probability.md) $p=3/4$ and $q=1/4$ gives joint [probabilities](probability.md) $3/16,9/16,1/16,3/16$ for $(H,H),(H,T),(T,H),(T,T)$. The row player's [expected payoff](expected-payoff.md) is $(3-9-1+3)/16=-1/4$, and the column player's is $1/4$.

Randomization can prevent an opponent exploiting a predictable choice. It does not mean every choice is equally good against every opponent: only [best responses](best-response.md) belong in the [support of a mixed strategy](support-of-a-mixed-strategy.md) at a [Nash equilibrium](nash-equilibrium.md). A shared random signal can instead produce a [lottery over joint action profiles](lottery-over-joint-action-profiles.md) whose joint [probabilities](probability.md) do not factor into [independent](independent-random-variables.md) [mixed strategies](mixed-strategy.md).

**Table of contents**

- [Support of a mixed strategy](support-of-a-mixed-strategy.md)
- [Strategy support](strategy-support.md)

## ↑ Ancestors (5)

1. [Game theory](game-theory-split.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (57)

- [Asymmetric coordination example](asymmetric-coordination-example.md)
- [Best response](best-response.md)
- [Brouwer gain-map proof of bimatrix equilibrium](brouwer-gain-map-proof-of-bimatrix-equilibrium.md)
- [Equilibrium preservation under iterated weak dominance](equilibrium-preservation-under-iterated-weak-dominance.md)
- [Expected payoff](expected-payoff.md)
- [Gain-map proof of symmetric equilibrium](gain-map-proof-of-symmetric-equilibrium.md)
- [Game theory](game-theory-split.md)
- [Lottery over joint action profiles](lottery-over-joint-action-profiles.md)
- [Marginal-equivalent equilibria in additive contests](marginal-equivalent-equilibria-in-additive-contests.md)
- [Minimax theorem](minimax-theorem.md)
- [Mixed strategy](mixed-strategy.md)
- [Nash equilibrium](nash-equilibrium.md)
- [Nash's theorem](nash-s-theorem.md)
- [Nondegeneracy of a bimatrix game](nondegeneracy-of-a-bimatrix-game.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-37/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-37/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-37/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-40/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/20c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-42/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-39/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/8h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-212/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/21h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/12g/c/solution.md)
- [Payoff matrix](payoff-matrix.md)
- [Positive-payoff linear programming for a matrix game](positive-payoff-linear-programming-for-a-matrix-game.md)
- [Prisoner's dilemma](prisoner-s-dilemma.md)
- [Replicator equation](replicator-equation.md)
- [Rock paper scissors](rock-paper-scissors.md)
- [Strategy profile](strategy-profile.md)
- [Strategy support](strategy-support.md)
- [Subgame perfect equilibrium](subgame-perfect-equilibrium.md)
- [Support certificate for an antisymmetric matrix game](support-certificate-for-an-antisymmetric-matrix-game.md)
- [Symmetric Nash equilibrium](symmetric-nash-equilibrium.md)
- [Unilateral deviation](unilateral-deviation.md)
- [Value of a zero-sum game](value-of-a-zero-sum-game.md)
- [Zero-sum game](zero-sum-game.md)
