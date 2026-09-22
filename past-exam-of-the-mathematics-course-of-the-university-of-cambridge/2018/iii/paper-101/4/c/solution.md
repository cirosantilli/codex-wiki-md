<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes.** Taking the constant coefficient defines a surjective [ring homomorphism](../../../../../../ring-homomorphism.md)

$$
\epsilon:R[[x]]\longrightarrow R,\qquad
\sum_{n\geq0}a_nx^n\longmapsto a_0.
$$

Its [kernel of a ring homomorphism](../../../../../../kernel-of-a-ring-homomorphism.md) is $(x)$, so the [first isomorphism theorem for rings](../../../../../../first-isomorphism-theorem-for-rings.md) gives $R[[x]]/(x)\cong R$.

We prove the needed preservation result. If $A$ is a [Noetherian ring](../../../../../../noetherian-ring.md) and $J\subseteq A$ is an [ideal](../../../../../../ideal.md), any ascending chain of [ideals](../../../../../../ideal.md) in $A/J$ lifts under the quotient [ring homomorphism](../../../../../../ring-homomorphism.md) to an ascending chain of [ideals](../../../../../../ideal.md) in $A$. The lifted chain stabilizes; surjectivity makes the original chain stabilize as well. Hence every [quotient ring](../../../../../../quotient-ring.md) of a [Noetherian ring](../../../../../../noetherian-ring.md) is [Noetherian](../../../../../../noetherian-ring.md).

Applying this with $A=R[[x]]$ and $J=(x)$ gives

$$
\boxed{R[[x]]\text{ Noetherian}\ \Longrightarrow\ R\text{ Noetherian}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
