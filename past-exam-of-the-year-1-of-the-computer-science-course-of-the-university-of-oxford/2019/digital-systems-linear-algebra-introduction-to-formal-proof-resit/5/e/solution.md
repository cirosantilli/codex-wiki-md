<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $r=\operatorname{rank}(A)$. If $r=0$, the [matrix](../../../../../matrix.md) is zero and the identity is immediate. Otherwise choose the [rank factorization](../../../../../rank-factorization.md) $A=BC$ from part b. The [column space](../../../../../column-space.md) of $B$ is the image of $A$.

An [idempotent matrix](../../../../../idempotent-matrix.md) acts as the identity on its image: if $u=Av$, then $Au=A^2v=Av=u$. Applying this to each column of $B$ gives $AB=B$. Substituting $A=BC$ yields $B(CB-I_r)=0$. Since $B$ has [full column rank](../../../../../full-column-rank.md), the represented map is injective, so each column of $CB-I_r$ is zero. Thus $CB=I_r$.

Now the rectangular [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md) gives

$$
\operatorname{tr}(A)=\operatorname{tr}(BC)=\operatorname{tr}(CB)
=\operatorname{tr}(I_r)=r=\operatorname{rank}(A).
$$

This proves that the [trace of an idempotent equals its rank](../../../../../trace-of-an-idempotent-equals-its-rank.md) using the supplied factorization method. Orthogonality of the projection is unnecessary: the argument applies to every real idempotent [matrix](../../../../../matrix.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
