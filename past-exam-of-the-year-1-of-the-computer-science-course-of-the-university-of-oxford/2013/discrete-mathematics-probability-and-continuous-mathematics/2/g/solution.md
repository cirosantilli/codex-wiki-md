<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

[Repeated squaring](../../../../../exponentiation-by-squaring.md) computes $a,a^2,a^4,a^8,\ldots$ by successively squaring. The [binary representation](../../../../../binary-number.md) of the exponent specifies which of these values to multiply. For [modular exponentiation](../../../../../modular-exponentiation.md), reduce after every multiplication; only a number of steps proportional to the [logarithm](../../../../../logarithm.md) of the exponent is needed.

Here $13\equiv2\pmod{11}$ and $17=16+1$. Successive squares give

$$
2^2\equiv4,\quad2^4\equiv16\equiv5,\quad2^8\equiv25\equiv3,\quad2^{16}\equiv9\pmod{11}.
$$

Therefore

$$
\boxed{13^{17}\equiv2^{16}2\equiv9\cdot2\equiv7\pmod{11};\quad\text{remainder }7.}
$$

## ↑ Ancestors (12)

1. [G](../g.md)
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
