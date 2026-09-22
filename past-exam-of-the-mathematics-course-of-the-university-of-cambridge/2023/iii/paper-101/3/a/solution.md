<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Zariski lemma](../../../../../../zariski-s-lemma.md) says that a field which is a [finitely generated algebra](../../../../../../finitely-generated-algebra.md) over a field $k$ is a finite algebraic extension of $k$. The [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md) says that, for an ideal $I\subseteq k[T_1,\ldots,T_n]$ over an [algebraically closed field](../../../../../../algebraically-closed-field.md),

$$
I(V(I))=\sqrt I.
$$

Let the unique point of $V(\mathfrak a)$ be $x=(x_1,\ldots,x_n)$ and let

$$
\mathfrak m=(T_1-x_1,\ldots,T_n-x_n).
$$

The Nullstellensatz gives $\sqrt{\mathfrak a}=\mathfrak m$, so $\mathfrak a\subseteq\mathfrak m$. Each of the finitely many generators $u_i=T_i-x_i$ of $\mathfrak m$ has some power $u_i^{e_i}\in\mathfrak a$. If

$$
r=1+\sum_i(e_i-1),
$$

then every monomial of total degree $r$ in the $u_i$ is divisible by one of the $u_i^{e_i}$. Hence

$$
\mathfrak m^r\subseteq\mathfrak a\subseteq\mathfrak m.
$$

**Thus the assertion is true; algebraically, the quotient defines a [punctual scheme](../../../../../../punctual-scheme.md) supported at $x$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
