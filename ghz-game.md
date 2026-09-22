# GHZ game

↑ **Parent:** [GHZ theorem](ghz-theorem.md)

A three-party [nonlocal game](nonlocal-game.md) with binary questions of even [Hamming weight](hamming-weight.md). Its winning output parity is half the question weight modulo two. For the four possible input triples, a hypothetical deterministic classical response would give four parity equations whose left sides cancel under [exclusive or](exclusive-or.md), while their right sides have odd total parity. Thus no classical strategy succeeds on every allowed triple, even with pre-shared randomness.

On the [GHZ state](greenberger-horne-zeilinger-state.md), measure the [Pauli X gate](pauli-x-gate.md) as an observable for question zero and the [Pauli Y gate](pauli-y-gate.md) for question one, and encode the measured [eigenvalue](eigenvalue.md) as $(-1)^x$. The joint observables XXX, XYY, YXY and YYX have respective GHZ [eigenvalues](eigenvalue.md) $+1,-1,-1,-1$. Their products of local outcomes enforce the required parity with certainty. The strategy uses pre-shared [quantum entanglement](entangled-state.md) and local measurements during the game, without communication. It realizes the [GHZ theorem](ghz-theorem.md) as an operational task. If the four questions are uniform, the best classical success is $3/4$: the parity contradiction bounds it above, and the deterministic rule $x=a$, $y=z=0$ wins three triples and loses only 011. The uniformity assumption is necessary for that numerical score, not for the impossibility of worst-case certainty.

## ↑ Ancestors (8)

1. [GHZ theorem](ghz-theorem.md)
2. [Greenberger–Horne–Zeilinger state](greenberger-horne-zeilinger-state.md)
3. [Controlled-NOT gate](controlled-not-gate.md)
4. [Controlled unitary gate](controlled-unitary-gate.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Nonlocal game](nonlocal-game.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/2/c/solution.md)
