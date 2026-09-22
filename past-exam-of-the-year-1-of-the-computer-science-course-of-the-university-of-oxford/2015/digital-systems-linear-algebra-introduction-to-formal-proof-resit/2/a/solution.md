<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [CMOS inverter](../../../../../cmos-inverter.md), connect one [PMOS transistor](../../../../../pmos-transistor.md) from the positive supply $V_{DD}$ to the output and one [NMOS transistor](../../../../../nmos-transistor.md) from the output to ground; drive both gates with the input $x$. When $x=0$, the [PMOS transistor](../../../../../pmos-transistor.md) conducts and the [NMOS transistor](../../../../../nmos-transistor.md) is off; when $x=1$, the reverse holds. Thus the output is $\neg x$, using two [transistors](../../../../../transistor.md).

For a four-input [NAND gate](../../../../../nand-gate.md), use four [NMOS transistors](../../../../../nmos-transistor.md) in series between the output and ground, with gates $a,b,c,d$. Use four [PMOS transistors](../../../../../pmos-transistor.md) in parallel between $V_{DD}$ and the output, with the same gate signals. The [pull-down network](../../../../../pull-down-network.md) conducts exactly when all four inputs are one; the [pull-up network](../../../../../pull-up-network.md) conducts whenever at least one input is zero. Hence

$$
\boxed{y=\neg(a\land b\land c\land d),\qquad N=8\text{ transistors}.}
$$

As usual for static [CMOS](../../../../../cmos.md), tie the [NMOS transistor](../../../../../nmos-transistor.md) bodies to ground and the [PMOS transistor](../../../../../pmos-transistor.md) bodies to $V_{DD}$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
