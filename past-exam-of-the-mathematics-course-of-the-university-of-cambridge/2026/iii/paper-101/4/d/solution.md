<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Work modulo $I$. Put

$$
C=R/(I+J),
$$

and let $A$ be the image of $I'/I$ in $C$. The separating condition $I'=I'\cap(I+J)$ modulo $I$ says that $I'/I\to C$ is injective, so we may regard $A$ as a submodule of $C$.

Since $r\in\sqrt{(I:I')}$, some power $r^q$ annihilates $A$. Apply the [Artin-Rees lemma](../../../../../../artin-rees-lemma.md) to $A\subseteq C$ and the principal ideal $(r)$. There is $s$ such that for every $m\ge s$,

$$
A\cap r^mC=r^{m-s}(A\cap r^sC).
$$

For $m\ge s+q$, the right side is zero. Pulling the equality $A\cap r^mC=0$ back to $R$ gives

$$
I'\cap(I+J+(r^m))=I,
$$

as required.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
