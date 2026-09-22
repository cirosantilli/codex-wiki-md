<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

A general binary [feedback shift register](../../../../../feedback-shift-register.md) of length $d$ has state

$$
(x_n,x_{n+1},\ldots,x_{n+d-1})\in\mathbb F_2^d
$$

and a feedback function $F:\mathbb F_2^d\to\mathbb F_2$. One update outputs the oldest bit, shifts the state, and inserts

$$
x_{n+d}=F(x_n,\ldots,x_{n+d-1}).
$$

The initial fill is $(x_0,\ldots,x_{d-1})$. It is a [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) when

$$
F(z_0,\ldots,z_{d-1})
=c_0z_0+\cdots+c_{d-1}z_{d-1}
$$

for fixed $c_i\in\mathbb F_2$.

The [Berlekamp-Massey algorithm](../../../../../berlekamp-massey-algorithm.md) reads an intercepted sequence from left to right while maintaining the shortest connection polynomial that reproduces the prefix. At each new symbol it computes the discrepancy between the observed bit and that predicted by the current recurrence. A zero discrepancy leaves the polynomial unchanged; a nonzero discrepancy adds a suitably shifted copy of the connection polynomial saved at the previous increase in linear complexity. After at least twice the unknown register length, it recovers the shortest recurrence, after which the entire keystream can be predicted.

Applying those discrepancy updates to

$$
1,1,0,0,1,0,1,1
$$

returns the connection polynomial

$$
\boxed{C(D)=1+D^2+D^3}.
$$

Equivalently, the sequence obeys

$$
\boxed{x_n=x_{n-2}+x_{n-3}\pmod2\qquad(n\geq3)}.
$$

Indeed this predicts successively $0,1,0,1,1$. No recurrence of length one or two fits the prefix, so its linear complexity is three.

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
