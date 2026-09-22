<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Replace the one-place marker $\mathrm{Empty}$ by three nullary [planning fluents](../../../../../planning-fluent.md) $q_0,q_1,q_2$, meaning that zero, one or two items are aboard. Initially only $q_0$ is true. Exactly one of these facts is maintained. No additional object constants are needed.

For compactness, define the common loading [preconditions](../../../../../precondition.md)

$$
L(x,s)=\{\mathrm{isItem}(x),\mathrm{isBank}(s),
\mathrm{at}(x,s),\mathrm{at}(\mathrm{BOAT},s)\}
$$

and common unloading [preconditions](../../../../../precondition.md)

$$
U(x,s)=\{\mathrm{isItem}(x),\mathrm{isBank}(s),
\mathrm{onBoat}(x),\mathrm{at}(\mathrm{BOAT},s)\}.
$$

The four [STRIPS](../../../../../strips.md) actions are

$$
\begin{aligned}
\mathrm{LoadFirst}(x,s):\quad
P&=L(x,s)\cup\{q_0\},\\
A&=\{\mathrm{onBoat}(x),q_1\},&
D&=\{\mathrm{at}(x,s),q_0\};\\[3pt]
\mathrm{LoadLast}(x,s):\quad
P&=L(x,s)\cup\{q_1\},\\
A&=\{\mathrm{onBoat}(x),q_2\},&
D&=\{\mathrm{at}(x,s),q_1\};\\[3pt]
\mathrm{UnloadFirst}(x,s):\quad
P&=U(x,s)\cup\{q_2\},\\
A&=\{\mathrm{at}(x,s),q_1\},&
D&=\{\mathrm{onBoat}(x),q_2\};\\[3pt]
\mathrm{UnloadLast}(x,s):\quad
P&=U(x,s)\cup\{q_1\},\\
A&=\{\mathrm{at}(x,s),q_0\},&
D&=\{\mathrm{onBoat}(x),q_1\}.
\end{aligned}
$$

Here the first unloading removes one of two items, and the last unloading removes the sole remaining item; items do not require fixed seat identities. The movement action remains as repaired in part (a) and changes none of the occupancy facts.

The [planning state invariant](../../../../../planning-state-invariant.md) is $q_j$ true exactly when $j$ items are aboard. Every action changes the marker by the same amount as the actual onboard count, so it follows by [mathematical induction](../../../../../mathematical-induction.md) from the initial empty boat. In particular, a third load is impossible.

## ↑ Ancestors (11)

1. [E](../e.md)
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
