<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [Euclidean algorithm](../../../../../../euclidean-algorithm.md) to $19$ and $11$:

$$
19=11+8,\quad 11=8+3,\quad 8=2\cdot3+2,\quad 3=2+1.
$$

Back-substitution gives the [Bézout's identity](../../../../../../bezout-s-identity.md)

$$
1=3-2=3\cdot3-8=3\cdot11-4\cdot8=7\cdot11-4\cdot19.
$$

Thus $(x,y)=(-4,7)$ is one solution of the [Diophantine equation](../../../../../../diophantine-equation.md). Subtracting this solution from any other gives

$$
19(x+4)+11(y-7)=0.
$$

Since $19$ and $11$ are [coprime](../../../../../../coprime-integers.md), $11$ divides $x+4$. To justify that step directly, multiply $1=-4\cdot19+7\cdot11$ by $x+4$: both terms on the right are divisible by $11$, because $19(x+4)=-11(y-7)$. Write $x+4=11t$; substitution then gives $y-7=-19t$. Therefore the complete solution set is

$$
\boxed{x=-4+11t,\qquad y=7-19t,\qquad t\in\mathbb Z.}
$$

Every such pair satisfies the original [Diophantine equation](../../../../../../diophantine-equation.md), since the $t$ terms cancel.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
