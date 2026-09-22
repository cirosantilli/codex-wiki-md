<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Every [complement of a set](../../../../../../complement-of-a-set.md) is taken in the same [universal set](../../../../../../universal-set.md) $\mathcal U$. Apply [De Morgan's laws](../../../../../../de-morgan-s-laws.md) for [propositional logic](../../../../../../propositional-logic.md) to the membership propositions. For every $x\in\mathcal U$,

$$
\begin{aligned}
x\in\overline{A\cap B}
&\iff\neg(x\in A\land x\in B)\\
&\iff(x\notin A\lor x\notin B)
\iff x\in\overline A\cup\overline B,\\
x\in\overline{A\cup B}
&\iff\neg(x\in A\lor x\in B)\\
&\iff(x\notin A\land x\notin B)
\iff x\in\overline A\cap\overline B.
\end{aligned}
$$

Equality of membership for every element proves the [set identities](../../../../../../set-identity.md)

$$
\boxed{\overline{A\cap B}=\overline A\cup\overline B,
\qquad\overline{A\cup B}=\overline A\cap\overline B.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
