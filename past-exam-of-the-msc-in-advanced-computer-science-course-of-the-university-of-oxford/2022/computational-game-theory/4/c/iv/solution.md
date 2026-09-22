<h1 id="4/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**No.** The denominator test from part ii is satisfied here, so a stronger obstruction is needed. Put $a_i=v(\{i\})$ and $b_{ij}=v(\{i,j\})$. In a three-player [simple cooperative game](../../../../../../simple-cooperative-game.md), the [Shapley value](../../../../../../shapley-value.md) formula gives, for distinct $i,j,k$,

$$
\phi_i=\frac13a_i+\frac16(b_{ij}-a_j)+\frac16(b_{ik}-a_k)+\frac13(1-b_{jk}).
$$

Subtract the corresponding expression for $\phi_j$:

$$
\phi_i-\phi_j=\frac12\bigl(a_i-a_j+b_{ik}-b_{jk}\bigr).
$$

Each [coalition](../../../../../../coalition-game-theory.md) value is zero or one, so this difference must be an integer multiple of $1/2$. This is the obstruction from [pairwise Shapley differences in a three-player simple game](../../../../../../pairwise-shapley-differences-in-a-three-player-simple-game.md). The proposed first two coordinates differ by $1/6$, which is not an integer multiple of $1/2$. Therefore the vector cannot occur, even though each coordinate separately passes the $1/6$ denominator test.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Computational game theory](../../../../computational-game-theory-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../../split.md)
7. [MSc in advanced computer science course of the University of Oxford](../../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
8. [Master's course of the University of Oxford](../../../../../../master-s-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
