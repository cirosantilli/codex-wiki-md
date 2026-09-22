<h1 id="12k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [discrete logarithm problem](../../../../../../discrete-logarithm-problem.md) asks, given $g$ and $h\equiv g^a\pmod p$, to recover $a$ modulo $p-1$. In the [Diffie-Hellman key exchange](../../../../../../diffie-hellman-key-exchange.md), Alice sends $g^a$, Bob sends $g^b$, and both compute $g^{ab}$. An enemy able to compute discrete logarithms recovers $a$ or $b$ from the public messages and hence obtains the key.

For three participants with private exponents $a,b,c$, circulate three tokens around a directed ring. Start with $g^a,g^b,g^c$; whenever a participant receives a token, they raise it to their private exponent and pass it on. Arrange the three cyclic routes so that after two transmissions each participant receives one token to which all three exponents have been applied. Every participant then has

$$
g^{abc},
$$

while the public transcript contains only proper subproducts.

For $n$ participants, start token $g^{a_i}$ at participant $i$ and pass it successively through the other $n-1$ participants in cyclic order, each raising it to their exponent. Choose the cyclic starts so that one completed token ends at each participant. Every final token equals

$$
g^{a_1a_2\cdots a_n}.
$$

There are $n$ tokens and $n-1$ transmissions per token, for exactly

$$
\boxed{n(n-1)=n^2-n}
$$

communications. Security rests on the corresponding generalized Diffie--Hellman problem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12K](../../12k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
