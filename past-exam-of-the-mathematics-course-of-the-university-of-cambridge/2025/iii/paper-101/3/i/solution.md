<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an ideal $I\subseteq k[T_1,\ldots,T_n]$, define

$$
V(I)=\{a\in k^n:f(a)=0\text{ for every }f\in I\}.
$$

For $X\subseteq k^n$, define

$$
I(X)=\{f:f(a)=0\text{ for every }a\in X\},
$$

and recall that $\sqrt I=\{f:f^r\in I\text{ for some }r\geq1\}$ is the [radical of an ideal](../../../../../../radical-of-an-ideal.md).

For an [algebraically closed field](../../../../../../algebraically-closed-field.md) $k$, the [Weak Hilbert Nullstellensatz](../../../../../../weak-hilbert-nullstellensatz.md) says that every maximal ideal of $k[T_1,\ldots,T_n]$ is

$$
(T_1-a_1,\ldots,T_n-a_n)
$$

for a unique $a\in k^n$, equivalently every proper ideal has a common zero. The [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md) says

$$
\boxed{I(V(I))=\sqrt I}.
$$

To prove the weak form, let $\mathfrak m$ be maximal. The residue field

$$
K=k[T_1,\ldots,T_n]/\mathfrak m
$$

is a field finitely generated as a $k$-algebra. By the [Zariski lemma](../../../../../../zariski-s-lemma.md), $K/k$ is finite algebraic; algebraic closedness gives $K=k$. If $a_i$ is the image of $T_i$, the quotient map is evaluation at $a=(a_1,\ldots,a_n)$ and its kernel is $(T_1-a_1,\ldots,T_n-a_n)$. This proves the assertion.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
