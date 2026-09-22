<h1 id="3g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Diffie-Hellman key exchange](../../../../../../diffie-hellman-key-exchange.md), Alice and Bob publicly agree on a cyclic group $G=\langle g\rangle$ in which the [discrete logarithm problem](../../../../../../discrete-logarithm-problem.md) is believed hard. Alice chooses a secret $a$ and sends $A=g^a$; Bob chooses a secret $b$ and sends $B=g^b$. They independently compute

$$
B^a=(g^b)^a=g^{ab}=(g^a)^b=A^b.
$$

Thus

$$
\boxed{K=g^{ab}}
$$

is their shared key. A passive eavesdropper sees $g,g^a,g^b$ but is believed unable to compute $g^{ab}$ efficiently; this is the computational Diffie--Hellman assumption. The basic protocol does not authenticate the participants and is therefore vulnerable to a man-in-the-middle attack unless the exchanged values are authenticated.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3G](../../3g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
