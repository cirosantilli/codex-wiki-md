<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each parenthesized pair in the given [Boolean function](../../../../../boolean-function.md) tests equality of two input [bits](../../../../../bit.md):

$$
(a\lor\neg c)\land(\neg a\lor c)=(a\land c)\lor(\neg a\land\neg c).
$$

This is [logical equivalence](../../../../../logical-equivalence.md), or the two-input [XNOR gate](../../../../../xnor-gate.md) function. Thus $z$ is one whenever either input pair agrees. Generate the four complemented inputs with four [inverters](../../../../../not-gate.md), and define the following [NAND gate](../../../../../nand-gate.md) outputs:

$$
\begin{aligned}
u_1&=\operatorname{NAND}(a,c),&u_2&=\operatorname{NAND}(\neg a,\neg c),\\
u_3&=\operatorname{NAND}(b,d),&u_4&=\operatorname{NAND}(\neg b,\neg d).
\end{aligned}
$$

Feed these four outputs into a single four-input [NAND gate](../../../../../nand-gate.md). [De Morgan's laws](../../../../../de-morgan-s-laws.md) give

$$
\boxed{z=\operatorname{NAND}(u_1,u_2,u_3,u_4)
=ac\lor\neg a\neg c\lor bd\lor\neg b\neg d.}
$$

Here juxtaposition denotes [logical conjunction](../../../../../logical-conjunction.md). The construction uses only [inverters](../../../../../not-gate.md), two-input [NAND gates](../../../../../nand-gate.md) and one four-input [NAND gate](../../../../../nand-gate.md), as required.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
