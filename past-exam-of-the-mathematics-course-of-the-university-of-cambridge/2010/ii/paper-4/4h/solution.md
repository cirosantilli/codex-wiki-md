<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

In a specified finite [cyclic group](../../../../../cyclic-group.md) $G=\langle g\rangle$, the [discrete logarithm problem](../../../../../discrete-logarithm-problem.md) is to recover $a$ modulo $|G|$ from $g$ and $g^a$. A common choice is a large prime-order subgroup of a [multiplicative group of a finite field](../../../../../multiplicative-group-of-a-finite-field.md).

For [Diffie-Hellman key exchange](../../../../../diffie-hellman-key-exchange.md), Alice and Bob independently choose private exponents $a,b$, transmit $g^a,g^b$, and compute respectively $(g^b)^a$ and $(g^a)^b$. Both obtain

$$
\boxed{K=g^{ab}.}
$$

Solving a [discrete logarithm problem](../../../../../discrete-logarithm-problem.md) reveals a private exponent and breaks this exchange. The converse implication is not known in general: recovering $g^{ab}$ from $g^a,g^b$ is the computational Diffie–Hellman problem, rather than literally the same task as computing a logarithm.

The advantage is that parties without an already shared secret can establish a fresh session key, which can then be used with efficient symmetric encryption. A classical secret-key system requires an earlier secure key distribution; ordinary public-key encryption can instead transmit a chosen key, but ephemeral [Diffie-Hellman key exchange](../../../../../diffie-hellman-key-exchange.md) also permits forward secrecy when private session exponents are erased and the exchange is authenticated. Authentication is essential: an unauthenticated exchange is vulnerable to a man-in-the-middle attack.

For [multilateral Diffie-Hellman key exchange](../../../../../multilateral-diffie-hellman-key-exchange.md) with $n$ participants with private exponents $a_1,\ldots,a_n$, send $n$ tokens clockwise around a ring. Participant $j$ starts the token $g^{a_j}$ and sends it to participant $j+1$. On each subsequent receipt, the receiver raises the token to their own private exponent and sends it onwards, until that token has made $n-1$ transmissions and reaches participant $j-1$. Its exponent then contains every exponent except $a_{j-1}$. The receiver raises it to $a_{j-1}$ locally, obtaining

$$
\boxed{K=g^{a_1a_2\cdots a_n}.}
$$

Every participant receives one such final token. There are $n$ tokens with exactly $n-1$ transmitted group elements per token, giving **$n(n-1)$ transmissions**. No private exponent is transmitted.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
