<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The source's system called $K$ already contains [positive introspection](../../../../../positive-introspection.md), so its displayed axioms are those usually called $K4$. Put

$$
B=\square(\square X\to X),\qquad A=(B\to\square X).
$$

We first show that its axioms prove $\square A\to A$, the implication suggested in the hint. From $B$, [positive introspection](../../../../../positive-introspection.md) gives $\square B$. Distribution applied to $\square A=\square(B\to\square X)$ and $\square B$ gives $\square\square X$. Distribution applied to $B=\square(\square X\to X)$ and this last result gives $\square X$. Thus the theorem-level implications combine by propositional reasoning into

$$
K4\vdash\square A\to(B\to\square X),
$$

which is $K4\vdash\square A\to A$.

Since $S$ contains these axioms, it proves that implication. Its assumed Löb [inference rule](../../../../../inference-rule.md), applied to the [first-order sentence](../../../../../first-order-sentence.md) $A$, yields $S\vdash A$. Unpacking $A$ proves

$$
\boxed{S\vdash\square(\square X\to X)\to\square X.}
$$

This uses necessitation only as part of the ordinary modal theorem rules; no inference of a boxed [temporary assumption](../../../../../temporary-assumption.md) has been made.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
