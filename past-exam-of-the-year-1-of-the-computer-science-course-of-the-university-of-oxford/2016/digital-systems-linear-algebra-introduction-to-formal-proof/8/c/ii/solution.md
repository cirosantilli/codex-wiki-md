<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For transitivity of [first-order equality](../../../../../../logical-equality.md), take the substitution formula $\phi(u)\equiv(T_1=u)$:
```
1  T₁ = T₂  premise
2  T₂ = T₃  premise
3  T₁ = T₃  =-elim 2,1; φ(u) := (T₁ = u)
```
For symmetry, use reflexivity and $\psi(u)\equiv(u=T_1)$:
```
1  T₁ = T₂  premise
2  T₁ = T₁  =-intro
3  T₂ = T₁  =-elim 1,2; ψ(u) := (u = T₁)
```
Thus **both transitivity and symmetry follow from the two equality rules**. In the symmetry proof, only the designated first occurrence in $T_1=T_1$ is replaced; the second remains fixed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
