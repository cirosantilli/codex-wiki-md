<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [STRIPS](../../../../../strips.md), a state records the true ground facts; under the [closed-world assumption](../../../../../closed-world-assumption.md), an absent fact is false. An action with positive [preconditions](../../../../../precondition.md) $P$, add effects $A$ and delete effects $D$ applies when $P\subseteq S$, producing $(S\setminus D)\cup A$.

The given movement action adds the destination fact without deleting the old boat location. After its first crossing the boat can therefore be recorded at both banks, allowing physically impossible loading. Its source-bank symbol is also not a declared action parameter. Repair both issues by using the fully parameterized [STRIPS](../../../../../strips.md) action

$$
\begin{aligned}
\mathrm{Move}(s,t):\quad
P&=\{\mathrm{isBank}(s),\mathrm{isBank}(t),
\mathrm{notEqual}(s,t),\mathrm{at}(\mathrm{BOAT},s)\},\\
A&=\{\mathrm{at}(\mathrm{BOAT},t)\},\\
D&=\{\mathrm{at}(\mathrm{BOAT},s)\}.
\end{aligned}
$$

Here $\mathrm{notEqual}(s,t)$ excludes a vacuous same-bank crossing. The two static inequality facts already supplied suffice.

The given loading action has no capacity check. Consecutive loads can put arbitrarily many items aboard. Introduce a nullary [planning fluent](../../../../../planning-fluent.md) $\mathrm{Empty}$, true initially, and repair loading to

$$
\begin{aligned}
\mathrm{Load}(x,s):\quad
P&=\{\mathrm{isItem}(x),\mathrm{isBank}(s),\mathrm{at}(x,s),
\mathrm{at}(\mathrm{BOAT},s),\mathrm{Empty}\},\\
A&=\{\mathrm{onBoat}(x)\},\\
D&=\{\mathrm{at}(x,s),\mathrm{Empty}\}.
\end{aligned}
$$

Unloading must restore $\mathrm{Empty}$, as in part (c). Including the bank $s$ explicitly as an action parameter removes the other unbound action variable. Equivalently, instantiate separate east-bank and west-bank actions.

These repairs establish the [planning state invariants](../../../../../planning-state-invariant.md) that the boat is at exactly one bank, each item is either at one bank or aboard, and at most one item is aboard. The first two hold initially and are preserved by deleting the former location when adding the new one; the capacity marker permits loading only when no item is aboard. Grounding implicit location variables alone would not repair the missing delete effect or the missing capacity check.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
