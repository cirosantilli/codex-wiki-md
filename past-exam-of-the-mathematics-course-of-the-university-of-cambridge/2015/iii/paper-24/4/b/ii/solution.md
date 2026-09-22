<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $M\subseteq N$ be transitive models of [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md) containing the set relation $R$ and its underlying set $X$. If $M$ judges $R$ well founded, it has an [ordinal rank function for a relation](../../../../../../../ordinal-rank-function-for-a-relation.md) $\rho\in M$ by the preceding rank characterization. Being a function to [ordinals](../../../../../../../ordinal.md) and satisfying

$$
\forall x,y\in X\ (xRy\Rightarrow\rho(x)<\rho(y))
$$

is absolute: the values are actual ordinals and the checks use only [bounded formulas in set theory](../../../../../../../bounded-formula-in-set-theory.md). The same rank function exists in $N$, so $N$ judges $R$ well founded.

Conversely, if $M$ judged it not well founded, it would contain a nonempty set $Y$ with no $R$-minimal element. The property of this particular $Y$ is bounded and remains true in $N$, contradicting well-foundedness there. Thus

$$
\boxed{M\models\text{“}R\text{ is well founded”}
\iff N\models\text{“}R\text{ is well founded”}.}
$$

This is [absoluteness of well-foundedness](../../../../../../../absoluteness-of-well-foundedness.md). The hypotheses that both models are transitive and satisfy [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md) matter; a small transitive set without sufficient recursion axioms need not contain the required rank witness.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
