<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A uniform witness can serve every particular input. Two [natural deduction](../../../../../natural-deduction.md) proofs differ in whether [universal introduction](../../../../../universal-quantifier-introduction-rule.md) happens outside or inside the existential witness box.
```
Proof 1:
1  ∃y ∀x R(x,y)      premise
2  | ∀x R(x,b)       assumption, b fresh
3  | R(a,b)          ∀-elim 2, with a arbitrary
4  | ∃y R(a,y)       ∃-intro 3
5  ∃y R(a,y)         ∃-elim 1,2–4
6  ∀x ∃y R(x,y)      ∀-intro 5

Proof 2:
1  ∃y ∀x R(x,y)      premise
2  | ∀x R(x,b)       assumption, b fresh
3  | R(a,b)          ∀-elim 2, with a arbitrary
4  | ∃y R(a,y)       ∃-intro 3
5  | ∀x ∃y R(x,y)    ∀-intro 4
6  ∀x ∃y R(x,y)      ∃-elim 1,2–5
```
In both proofs $a$ is absent from the original premise. In the second it is also absent from the witness assumption, whose $x$ is bound; universal generalization is therefore legal inside that box. The exported conclusions contain no free $b$.

The converse is **not valid**. On the domain $\{0,1\}$, interpret $R(x,y)$ as $x=y$. For each $x$, choose $y=x$, so $\forall x\exists yR(x,y)$ holds. Neither single choice of $y$ equals both 0 and 1, so $\exists y\forall xR(x,y)$ fails. This is the distinction between a [pointwise witness](../../../../../pointwise-witness.md) and a [uniform witness](../../../../../uniform-witness.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
