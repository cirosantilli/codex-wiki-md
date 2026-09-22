<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Write $F,R,C$ for the three item constants, $E,W$ for the banks, $L,U,M$ for the corrected load, unload and move actions, and $K_s$ for $\mathrm{Check}(s,p_F,p_R,p_C)$ instantiated with the items' actual current locations. A fully executable plan in the [STRIPS](../../../../../strips.md) model of part (g) is

$$
\begin{aligned}
&L(R,E),\ K_E,\ M(E,W),\ U(R,W),\\
&K_W,\ M(W,E),\\
&L(F,E),\ K_E,\ M(E,W),\ U(F,W),\\
&L(R,W),\ K_W,\ M(W,E),\ U(R,E),\\
&L(C,E),\ K_E,\ M(E,W),\ U(C,W),\\
&K_W,\ M(W,E),\\
&L(R,E),\ K_E,\ M(E,W),\ U(R,W).
\end{aligned}
$$

Thus the seven crossings carry **rabbit west, nothing east, fox west, rabbit east, carrot west, nothing east, rabbit west**.

Immediately before those crossings, the items left on the departure bank are respectively $\{F,C\},\{R\},\{C\},\{F\},\{R\},\{F,C\},\varnothing$. None contains an incompatible pair, so each displayed $K_s$ has its safety [preconditions](../../../../../precondition.md). Each loaded crossing carries exactly one item, and all three finish west.

## ↑ Ancestors (11)

1. [H](../h.md)
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
