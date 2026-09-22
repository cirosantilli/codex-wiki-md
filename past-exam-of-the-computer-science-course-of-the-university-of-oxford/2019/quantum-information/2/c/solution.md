<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For deterministic classical responses, denote the two possible local answers by $x_0,x_1$, $y_0,y_1$ and $z_0,z_1$. Certainty in the [GHZ game](../../../../../ghz-game.md) would require

$$
\begin{aligned}
x_0\oplus y_0\oplus z_0&=0,\\
x_0\oplus y_1\oplus z_1&=1,\\
x_1\oplus y_0\oplus z_1&=1,\\
x_1\oplus y_1\oplus z_0&=1.
\end{aligned}
$$

Taking the [exclusive or](../../../../../exclusive-or.md) of all four equations gives zero on the left, since every answer occurs twice, but one on the right. This contradiction rules out deterministic certainty. Pre-shared randomness cannot cure it: conditioning on the random seed fixes a deterministic response table, and none succeeds on every allowed input. Thus **noncommunicating classical players cannot win with certainty**. No uniform distribution on the referee's questions is needed for this worst-case claim.

For the quantum strategy, share the [GHZ state](../../../../../greenberger-horne-zeilinger-state.md) and measure the [Pauli X gate](../../../../../pauli-x-gate.md) observable when the local question is 0, or the [Pauli Y gate](../../../../../pauli-y-gate.md) observable when it is 1. Return bit 0 for measurement [eigenvalue](../../../../../eigenvalue.md) $+1$ and bit 1 for [eigenvalue](../../../../../eigenvalue.md) $-1$. The four relevant operator identities are

$$
\begin{aligned}
(X\otimes X\otimes X)|GHZ\rangle&=|GHZ\rangle,\\
(X\otimes Y\otimes Y)|GHZ\rangle&=-|GHZ\rangle,\\
(Y\otimes X\otimes Y)|GHZ\rangle&=-|GHZ\rangle,\\
(Y\otimes Y\otimes X)|GHZ\rangle&=-|GHZ\rangle.
\end{aligned}
$$

For the first identity, the three bit flips exchange $|000\rangle$ and $|111\rangle$. For each remaining identity, the two Y actions contribute $i^2=-1$ on $|000\rangle$ and $(-i)^2=-1$ on $|111\rangle$, so they exchange the terms with a minus sign. Local measurements on separate systems commute, and the product of their observed [eigenvalues](../../../../../eigenvalue.md) is therefore fixed by the displayed joint [eigenvalue](../../../../../eigenvalue.md). That product equals $(-1)^{x+y+z}$, giving exactly the required output parity for each promised input. Hence **the quantum strategy wins with certainty without communication**. This is the [GHZ theorem](../../../../../ghz-theorem.md) in nonlocal-game form; it does not let a player control another player's individual outcome.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
