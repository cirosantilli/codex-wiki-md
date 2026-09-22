<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $A_0=0$ and recursively set

$$
A_{n+1}-A_n
=\mathbb E[X_{n+1}-X_n\mid\mathcal F_n].
$$

The increment is $\mathcal F_n$-measurable, so $A_{n+1}$ is $\mathcal F_n$-measurable by induction; hence $A$ is [predictable](../../../../../../predictable-process.md). Conditional expectation preserves integrability, so $A_n$ and

$$
M_n=X_n-A_n
$$

are integrable and adapted. Their increments satisfy

$$
\mathbb E[M_{n+1}-M_n\mid\mathcal F_n]
=\mathbb E[X_{n+1}-X_n\mid\mathcal F_n]
-(A_{n+1}-A_n)=0,
$$

so $M$ is a martingale.

For uniqueness, suppose $X=M+A=M'+A'$ are two such decompositions. Then

$$
D=M-M'=A'-A
$$

is both a martingale and predictable, with $D_0=0$. Since $D_{n+1}$ is $\mathcal F_n$-measurable,

$$
D_{n+1}=\mathbb E[D_{n+1}\mid\mathcal F_n]=D_n.
$$

Induction gives $D=0$, and therefore $M=M'$ and $A=A'$. This proves the [Doob decomposition of an adapted integrable process](../../../../../../doob-decomposition-of-an-adapted-integrable-process.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
