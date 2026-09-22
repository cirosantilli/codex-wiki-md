<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Generate four partial-product [bits](../../../../../bit.md) with [AND gates](../../../../../and-gate.md):

$$
p_{00}=x_0y_0,\quad p_{10}=x_1y_0,\quad p_{01}=x_0y_1,\quad p_{11}=x_1y_1.
$$

The [binary multiplication](../../../../../binary-multiplication.md) expansion is $XY=p_{00}+2(p_{10}+p_{01})+4p_{11}$. Add the two weight-two [bits](../../../../../bit.md) with a [half adder](../../../../../half-adder.md), then add its [carry](../../../../../carry-arithmetic.md) to $p_{11}$ with a second [half adder](../../../../../half-adder.md). The complete [combinational logic](../../../../../combinational-logic.md) is

$$
\begin{aligned}
z_0&=p_{00},&z_1&=p_{10}\oplus p_{01},&c&=p_{10}\land p_{01},\\
z_2&=p_{11}\oplus c,&z_3&=p_{11}\land c.
\end{aligned}
$$

Thus **four [AND gates](../../../../../and-gate.md) for the partial products and two [half adders](../../../../../half-adder.md) suffice**. Each [half adder](../../../../../half-adder.md) contains one [exclusive or](../../../../../exclusive-or.md) gate and one [AND gate](../../../../../and-gate.md). In the largest case $3\times3=9$, these equations produce $1001$, including the necessary fourth output [bit](../../../../../bit.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
