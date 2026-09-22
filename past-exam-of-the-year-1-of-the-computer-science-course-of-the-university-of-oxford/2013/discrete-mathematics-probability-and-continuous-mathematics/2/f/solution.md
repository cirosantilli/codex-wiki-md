<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use [modular arithmetic](../../../../../modular-arithmetic-split.md) to keep all intermediate numbers small:

$$
34\equiv2,\quad45\equiv5,\quad55\equiv7,\quad89\equiv1\pmod8.
$$

Thus $34\cdot45\cdot55+89\equiv2\cdot5\cdot7+1=71\equiv7\equiv-1\pmod8$. Cubing gives

$$
\boxed{(34\cdot45\cdot55+89)^3\equiv(-1)^3\equiv7\pmod8;\quad\text{remainder }7.}
$$

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
