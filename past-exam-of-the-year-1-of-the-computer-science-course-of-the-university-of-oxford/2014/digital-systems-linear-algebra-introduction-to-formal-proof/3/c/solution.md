<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [synchronous counter cascade](../../../../../synchronous-counter-cascade.md), with the three-[bit](../../../../../bit.md) [modulo-six counter](../../../../../modulo-six-counter.md) advancing on every active [clock edge](../../../../../clock-edge.md) and the [Gray-code counter](../../../../../gray-code-counter.md) advancing only when the old binary state is $101$. Its enable can therefore be

$$
\boxed{E=A C.}
$$

On the six valid binary states, $AC=1$ only at $101$. Both [digital counters](../../../../../digital-counter.md) sample the same clock: at an edge leaving $101$, the binary output becomes $000$ and $GH$ simultaneously advances to the next [Gray code](../../../../../gray-code.md). At all other edges $GH$ holds. Starting from $GHABC=00000$, this gives exactly the listed 24-state sequence. Use the shared clock and an enable, rather than making a combinational terminal-state signal into a new clock.[Question 3(c), printed page 4: original 24-row state/output table](../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2014.md)

For the output $Y$, every state with $C=1$ has $Y=1$. For $C=0$, the only extra high states are $GH=01$ with binary state $010$, and $GH=11$ with binary state $000$ or $100$. On valid states these conditions are $H\overline G B$ and $HG\overline B$, respectively. Hence

$$
\boxed{Y=C+H\overline G B+HG\overline B=C\lor\bigl(H\land(G\mathbin{\oplus}B)\bigr).}
$$

The lower circuit in the figure implements this with an AND for $E$, an [exclusive or](../../../../../exclusive-or.md) on $G,B$, an AND with $H$, and an OR with $C$. The resulting [Morse code](../../../../../morse-code.md) output blocks, in [Gray code](../../../../../gray-code.md) order $00,01,11,10$, are

$$
010101\quad011101\quad110111\quad010101.
$$

Across the two middle blocks these join to three three-clock highs separated by one-clock lows; the first and last blocks provide the three single-clock highs of each S. The specified table is a repeating SOS symbol pattern; its wraparound has a one-clock low, rather than an added inter-message pause. The output is a [Moore machine](../../../../../moore-machine.md) decoding of current stored [bits](../../../../../bit.md); its value changes after those [bits](../../../../../bit.md) settle.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
