<h1 id="6c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taylor-expand the gain terms:

$$
\lambda P(n-1)
=\lambda\left(P-P_n+\frac12P_{nn}+\cdots\right),
$$

and, writing $Q(n)=\beta n^2P(n)$,

$$
Q(n+2)=Q+2Q_n+2Q_{nn}+\cdots.
$$

After cancellation of the loss terms, the second-order [Kramers-Moyal expansion](../../../../../../kramers-moyal-expansion.md) is

$$
\frac{\partial P}{\partial t}
=-\frac{\partial}{\partial n}
\left[(\lambda-2\beta n^2)P\right]
+\frac12\frac{\partial^2}{\partial n^2}
\left[(\lambda+4\beta n^2)P\right].
$$

Hence the [constant-birth pair-annihilation process](../../../../../../constant-birth-pair-annihilation-process.md) has

$$
\boxed{A(n)=\lambda-2\beta n^2},
\qquad
\boxed{B(n)=\lambda+4\beta n^2}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6C](../../6c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
