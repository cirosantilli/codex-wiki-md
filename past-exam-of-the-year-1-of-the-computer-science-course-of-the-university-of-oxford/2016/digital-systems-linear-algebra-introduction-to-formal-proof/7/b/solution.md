<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $H=(P\land Q)\lor(P\land R)$. In the following [natural deduction](../../../../../natural-deduction.md) proofs, indentation and vertical bars mark assumption scopes. Rule names are the introduction and elimination rules supplied by the paper.

First work backwards from the premise using [disjunction elimination](../../../../../disjunction-elimination-rule.md), proving the whole desired [logical conjunction](../../../../../logical-conjunction.md) in each case:
```
1  H               premise
 2  | P ∧ Q        assumption
 3  | P            ∧-elim-L 2
 4  | Q            ∧-elim-R 2
 5  | Q ∨ R        ∨-intro-L 4
 6  | P ∧ (Q ∨ R)  ∧-intro 3,5
 7  | P ∧ R        assumption (new case)
 8  | P            ∧-elim-L 7
 9  | R            ∧-elim-R 7
10  | Q ∨ R        ∨-intro-R 9
11  | P ∧ (Q ∨ R)  ∧-intro 8,10
12  P ∧ (Q ∨ R)    ∨-elim 1,2–6,7–11
```
Alternatively, first transform the goal by [conjunction introduction](../../../../../conjunction-introduction-rule.md), obtaining $P$ and $Q\lor R$ by separate [disjunction elimination](../../../../../disjunction-elimination-rule.md) proofs:
```
1  H             premise
 2  | P ∧ Q      assumption
 3  | P          ∧-elim-L 2
 4  | P ∧ R      assumption (new case)
 5  | P          ∧-elim-L 4
 6  P            ∨-elim 1,2–3,4–5
 7  | P ∧ Q      assumption
 8  | Q          ∧-elim-R 7
 9  | Q ∨ R      ∨-intro-L 8
10  | P ∧ R      assumption (new case)
11  | R          ∧-elim-R 10
12  | Q ∨ R      ∨-intro-R 11
13  Q ∨ R        ∨-elim 1,7–9,10–12
14  P ∧ (Q ∨ R)  ∧-intro 6,13
```
The essential difference is the final rule: the first proof splits the premise once, while the second splits the goal first and then analyzes the premise twice. Counting only rule applications, **both displayed proofs take nine inference steps**. The first uses four [conjunction elimination](../../../../../conjunction-elimination-rule.md) steps, two [disjunction introduction](../../../../../disjunction-introduction-rule.md) steps, two [conjunction introduction](../../../../../conjunction-introduction-rule.md) steps and one [disjunction elimination](../../../../../disjunction-elimination-rule.md); the second replaces one [conjunction introduction](../../../../../conjunction-introduction-rule.md) with a second [disjunction elimination](../../../../../disjunction-elimination-rule.md). If assumption lines are counted as displayed proof lines, the second is longer, 14 rather than 12, because it opens four case assumptions rather than two. Thus a raw line count and an inference-step count need not agree.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
