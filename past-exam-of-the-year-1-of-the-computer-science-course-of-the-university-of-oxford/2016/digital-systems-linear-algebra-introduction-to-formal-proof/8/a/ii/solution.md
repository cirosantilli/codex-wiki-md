<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a fresh parameter $a$. The [universal quantifier elimination rule](../../../../../../universal-quantifier-elimination-rule.md) supplies both the implication and its premise at that same parameter:
```
1  ∀x. (P(x) → Q(x))        premise
2  | ∀x. P(x)               assumption
3  | P(a)                   ∀-elim 2
4  | P(a) → Q(a)            ∀-elim 1
5  | Q(a)                   →-elim 4,3
6  | ∀x. Q(x)               ∀-intro 5, a fresh
7  (∀x. P(x)) → (∀x. Q(x))  →-intro 2–6
```
The [eigenvariable condition](../../../../../../eigenvariable-condition.md) holds because $a$ is absent from both undischarged assumptions at line 6. Hence **the universally quantified implication is proved**.

The proposed version with merely $P(x)$ in the antecedent is **not derivable**. For a [counterexample](../../../../../../counterexample.md), take a two-element domain $\{0,1\}$ with $P$ and $Q$ both true precisely at zero. The universal premise holds. Under the assignment $x=0$, $P(x)$ is true but $\forall x\,Q(x)$ is false. By [soundness](../../../../../../soundness.md), a formal proof cannot exist. Attempting the previous derivation would fail exactly at [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md): the parameter would occur in the undischarged assumption $P(x)$, so it would not be fresh.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
