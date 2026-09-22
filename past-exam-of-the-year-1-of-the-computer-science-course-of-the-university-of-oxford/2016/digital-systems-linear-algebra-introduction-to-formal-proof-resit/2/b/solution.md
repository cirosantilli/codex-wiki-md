<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Encode $(q_1q_0)$ by $A=00$, $B=01$, $C=11$, $I=10$, with reset to $A$. Two positive-edge-triggered [D flip-flops](../../../../../d-flip-flop.md) store the state. Minimizing the [Boolean functions](../../../../../boolean-function.md) from the complete table gives

$$
\boxed{D_0=x_0+q_0x_1,\qquad D_1=\bar x_0q_0(x_1+q_1),\qquad INC=q_1\bar q_0.}
$$

Equivalently, the minimal [sum of products](../../../../../disjunctive-normal-form.md) form of $D_1$ is $\bar x_0q_0x_1+\bar x_0q_0q_1$. The displayed factorization saves duplicated logic. The equations use only [AND gates](../../../../../and-gate.md), [OR gates](../../../../../or-gate.md) and [NOT gates](../../../../../not-gate.md); connect $D_j$ to the corresponding flip-flop data input and use one common clock.

For example, $C$ with input $00$ gives $(D_1D_0)=10$, entering the pulse state. In $I$, either $x_0=1$ gives $01$ or $x_0=0$ gives $00$, independently of $x_1$; the pulse cannot persist. The four states are distinguishable by their current output or future response to inputs $00$ and $10,00$, so two state bits are also necessary.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
