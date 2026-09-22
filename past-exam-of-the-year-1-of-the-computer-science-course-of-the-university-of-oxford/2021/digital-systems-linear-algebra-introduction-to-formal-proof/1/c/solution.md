<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $K=0$, a [JK flip-flop](../../../../../jk-flip-flop.md) obeys $Q^+=J\lor Q$ at its positive [clock edge](../../../../../clock-edge.md): $J=0$ holds its old state and $J=1$ sets it. Thus each original stage is a sticky record of a previously sampled high input until Start clears it. A [D flip-flop](../../../../../d-flip-flop.md) instead obeys $Q^+=D$, so a later sample of zero can clear the output.

Connect each replacement D input where the corresponding J input was connected, preserving the clocks and [asynchronous clear](../../../../../asynchronous-clear.md). The first valid sequence after Start still sets both outputs. Afterwards, let $X_0$ fall and apply another rising [clock edge](../../../../../clock-edge.md) to $X_1$. **The D version clears $Y_0$; the JK version retains $Y_0=1$.** A subsequent rising [clock edge](../../../../../clock-edge.md) of $X_2$ can therefore clear $Y_1$ only in the D version. Neither circuit continuously tracks its data input between [clock edges](../../../../../clock-edge.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
