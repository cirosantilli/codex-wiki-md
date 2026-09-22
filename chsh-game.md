# CHSH game

↑ **Parent:** [CHSH inequality](chsh-inequality.md)

Two separated players receive uniformly random input [bits](bit.md) $a,b$ and output [bits](bit.md) $x,y$ without communicating after receiving their inputs. They win when $x\oplus y=ab$, with [exclusive or](exclusive-or.md) $\oplus$. For deterministic local response functions, the four desired equalities have inconsistent parity, so at most three can hold. Shared randomness only averages such strategies, proving classical winning [probability](probability.md) at most $3/4$. In terms of correlations $E_{ab}=\mathbb E[(-1)^{x+y}\mid a,b]$, the winning [probability](probability.md) is $1/2+(E_{00}+E_{01}+E_{10}-E_{11})/8$, directly connecting the game to the [CHSH inequality](chsh-inequality.md).

## ↑ Ancestors (7)

1. [CHSH inequality](chsh-inequality.md)
2. [Bell theorem](bell-theorem.md)
3. [Foundations of quantum mechanics](foundations-of-quantum-mechanics-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information/1/c/ii/solution.md)
- [Reflected real-basis CHSH strategy](reflected-real-basis-chsh-strategy.md)
