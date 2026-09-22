<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After asserting and releasing the active-low Start pulse, a valid sequence is **$X_0\uparrow$, then $X_1\uparrow$, then $X_2\uparrow$**, with each input held high through the relevant sampling interval. The first [JK flip-flop](../../../../../jk-flip-flop.md) has $J=X_0,K=0$ and is clocked by $X_1$, so the rising [clock edge](../../../../../clock-edge.md) of $X_1$ samples $X_0=1$ and sets $Y_0=1$. Once that output has settled, a rising [clock edge](../../../../../clock-edge.md) of $X_2$ clocks the second [JK flip-flop](../../../../../jk-flip-flop.md) with $J=Y_0=1,K=0$, setting $Y_1=1$.

The essential conditions concern sampled levels: $X_0$ must be high at a rising [clock edge](../../../../../clock-edge.md) of $X_1$, and $Y_0$ must then be high at a rising [clock edge](../../../../../clock-edge.md) of $X_2$. Separate edges with adequate [setup and hold time](../../../../../setup-and-hold-time.md) avoid an ambiguous simultaneous transition.

## ↑ Ancestors (12)

1. [A](../a.md)
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
