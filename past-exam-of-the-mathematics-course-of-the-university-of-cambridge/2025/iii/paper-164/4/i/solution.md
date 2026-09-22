<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Entropic Balog-Szemerédi-Gowers theorem](../../../../../../entropic-balog-szemeredi-gowers-theorem.md) states that for finitely supported random variables $A,B$ in an [abelian group](../../../../../../abelian-group.md),

$$
d_R(A;B\mathbin\Vert A+B)
\leq3I(A;B)+2H(A+B)-H(A)-H(B),
$$

where the left-hand side is the [Simultaneous conditional entropic Ruzsa distance](../../../../../../simultaneous-conditional-entropic-ruzsa-distance.md).

Put $S=A+B$ and take two copies $(A_1,B_1)$ and $(A_2,B_2)$ that are conditionally independent given $S$. Thus both sums equal $S$, and, given $S$, $A_1$ and $B_2$ are independent with the required conditional marginals. By [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md),

$$
d_R(A;B\mathbin\Vert S)
\leq H(A_1-B_2)
-\frac12H(A_1\mid S)-\frac12H(B_2\mid S).
$$

The two conditional entropies are equal, since either $A$ or $B$ together with $S$ determines the other, and the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) gives

$$
H(A\mid S)=H(B\mid S)
=H(A)+H(B)-I(A;B)-H(S).
$$

Set $D=A_1-B_2$. By [entropy submodularity](../../../../../../entropy-submodularity.md),

$$
H(D)\leq H(D,A_1)+H(D,B_1)-H(D,A_1,B_1).
$$

The first term is $H(A_1,B_2)\leq H(A)+H(B)$ by [subadditivity of information entropy](../../../../../../subadditivity-of-information-entropy.md). Since $A_1+B_1=A_2+B_2$, we also have $D=A_2-B_1$, so the second term is at most $H(A)+H(B)$. Finally $(D,A_1,B_1)$ determines all four copied variables, and conditional independence gives

$$
\begin{aligned}
H(D,A_1,B_1)
&=H(A_1,B_1,A_2,B_2)\\
&=H(S)+2H(A,B\mid S)\\
&=2H(A,B)-H(S).
\end{aligned}
$$

As $H(A,B)=H(A)+H(B)-I(A;B)$, these estimates imply

$$
H(D)\leq H(S)+2I(A;B).
$$

Subtracting the common conditional-entropy term proves the stated [Entropic Balog-Szemerédi-Gowers theorem](../../../../../../entropic-balog-szemeredi-gowers-theorem.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
