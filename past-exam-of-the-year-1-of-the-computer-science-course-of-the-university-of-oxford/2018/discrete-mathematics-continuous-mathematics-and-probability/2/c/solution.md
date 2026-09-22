<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First prove $a^p\equiv a\pmod p$ for every [nonnegative integer](../../../../../natural-number.md) $a$ by [mathematical induction](../../../../../mathematical-induction.md). The case $a=0$ is immediate. If it holds at $a$, the [binomial theorem](../../../../../binomial-theorem.md) and the stated divisibility of the middle [binomial coefficients](../../../../../binomial-coefficient-split.md) give

$$
(a+1)^p\equiv a^p+1\equiv a+1\pmod p.
$$

This establishes the induction. For an arbitrary [integer](../../../../../integer-split.md) $a$, take a nonnegative representative $r$ of its [residue class](../../../../../residue-class.md); then $a^p\equiv r^p\equiv r\equiv a\pmod p$. When $a\not\equiv0\pmod p$, part (b) supplies a [multiplicative inverse](../../../../../multiplicative-inverse.md) modulo $p$. Multiplying the congruence by that inverse proves [Fermat's little theorem](../../../../../fermat-little-theorem.md):

$$
\boxed{a^{p-1}\equiv1\pmod p.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
