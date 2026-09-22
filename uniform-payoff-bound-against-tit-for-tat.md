# Uniform payoff bound against Tit for tat

↑ **Parent:** [Tit for tat](tit-for-tat.md)

In a symmetric two-action stage game write $R,P,T_{\rm tempt},S$ for mutual cooperation, mutual defection, sole defection and sole cooperation [payoffs](payoff.md). Suppose $T_{\rm tempt}\ge R$, $P\le R$ and $T_{\rm tempt}+S\le2R$. Against an initially cooperative [Tit for tat](tit-for-tat.md), every action [sequence](sequence.md) has limiting upper average [payoff](payoff.md) at most $R$.

For a deviator's actions $a_t$, put $a_{-1}=C$, $h(C)=0$ and $h(D)=T_{\rm tempt}-R$. The opponent at time $t$ plays $a_{t-1}$. Check the four transitions: $C$ to $C$ and $C$ to $D$ satisfy

$$
u(a_t,a_{t-1})\le R+h(a_t)-h(a_{t-1})
$$

with equality; $D$ to $C$ uses $S\le2R-T_{\rm tempt}$, and $D$ to $D$ uses $P\le R$. A [telescoping sum](telescoping-sum.md) gives the displayed finite-horizon bound. Divide by the horizon and let it increase. Mutual [Tit for tat](tit-for-tat.md) yields $R$ every round, so it is a [Nash equilibrium](nash-equilibrium.md) under the [long-run average payoff](long-run-average-payoff.md) criterion. The argument is pathwise and therefore covers arbitrary deviations representable by [finite-state machines](finite-state-machine.md), as well as action [sequences](sequence.md) outside that class.

## ↑ Ancestors (9)

1. [Tit for tat](tit-for-tat.md)
2. [Reactive strategy (game theory)](reactive-strategy-game-theory.md)
3. [Iterated prisoner's dilemma](iterated-prisoner-s-dilemma.md)
4. [Prisoner's dilemma](prisoner-s-dilemma.md)
5. [Game theory](game-theory-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/3/b/solution.md)
