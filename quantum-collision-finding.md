# Quantum collision finding

↑ **Parent:** [Quantum query complexity](quantum-query-complexity.md)

Given a [function](function-split.md) $f$ with an $m$-bit output, accessed through the [unitary operator](unitary-operator.md) $U_f|x\rangle|y\rangle=|x\rangle|y\mathbin\oplus f(x)\rangle$, quantum collision finding asks for distinct inputs with equal outputs. Here $\oplus$ is bitwise [exclusive or](exclusive-or.md) on the $m$-bit answer [quantum register](quantum-register.md). The distinctness requirement excludes the uninformative pair $(x,x)$. For a two-to-one function on $N$ inputs, [Grover search algorithm](grover-s-algorithm.md) methods yield a cube-root [quantum query complexity](quantum-query-complexity.md), despite a square-root cost for finding a partner of just one preselected input.

**Table of contents**

- [Brassard–Høyer–Tapp collision algorithm](brassard-hoyer-tapp-collision-algorithm.md)

## ↑ Ancestors (6)

1. [Quantum query complexity](quantum-query-complexity.md)
2. [Quantum complexity theory](quantum-complexity-theory.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Function collision](function-collision.md)
