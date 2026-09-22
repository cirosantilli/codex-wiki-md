<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

All calculations are in [modular arithmetic](../../../../../../modular-arithmetic-split.md) modulo $n$. Expand the two expressions appearing in the proposed quotient:

$$
\begin{aligned}
c_2+2c_1-1&\equiv(m+1)^3+2m^3-1\\
&=3m^3+3m^2+3m,\\
c_2-c_1+2&\equiv(m+1)^3-m^3+2\\
&=3m^2+3m+3.
\end{aligned}
$$

The first is exactly $m$ times the second. Multiplication by the assumed [modular multiplicative inverse](../../../../../../modular-multiplicative-inverse.md) therefore gives

$$
\boxed{m\equiv(c_2+2c_1-1)(c_2-c_1+2)^{-1}\pmod n.}
$$

The representative in $\{0,\ldots,n-1\}$ is the [plaintext](../../../../../../plaintext.md). This [RSA related-message attack](../../../../../../rsa-related-message-attack.md) uses a relation between messages to turn two cubic equations into a linear equation; it does not recover the [private key](../../../../../../private-key.md) or factor $n$ in the invertible case.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
