<h1 id="a/4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the supplied uniqueness theorem for the modalized [logical formula](../../../../../logical-formula.md) $A(p)=\Box p\to X$. Its occurrence of $p$ is boxed, and the source assumes $p$ does not occur in $X$. Choose another [first-order sentence](../../../../../first-order-sentence.md) letter $q$ absent from $X$ and from $p$. Besides the uniqueness theorem and propositional reasoning, use that GL is closed under [uniform substitution in modal logic](../../../../../uniform-substitution-in-modal-logic.md).

Let $Y=\Box X\to X$. Uniformly substitute $Y$ for the fresh letter $q$ in the uniqueness theorem. Since $q$ occurs nowhere in $X$, this gives

$$
GL\vdash\bigl(\Box(p\leftrightarrow(\Box p\to X))\wedge
\Box(Y\leftrightarrow(\Box Y\to X))\bigr)\to\Box(p\leftrightarrow Y).
$$

Part (c) proves the second conjunct outright. Propositional reasoning removes that already-proved conjunct and yields

$$
\boxed{GL\vdash\Box(p\leftrightarrow(\Box p\to X))\to
\Box(p\leftrightarrow(\Box X\to X)).}
$$

The freshness conditions make the substitution legal and ensure it changes only the placeholder intended for the second fixed point.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
