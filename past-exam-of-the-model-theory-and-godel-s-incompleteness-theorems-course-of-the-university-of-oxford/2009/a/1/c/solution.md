<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [consistency of a negated-consistency extension](../../../../../consistency-of-a-negated-consistency-extension.md), put $A=S+\neg\operatorname{Con}_S$. The [arithmetized deduction theorem](../../../../../arithmetized-deduction-theorem.md), together with double-negation elimination and formalized proof transformations, gives

$$
S\vdash\Box_A\bot\leftrightarrow\Box_S\operatorname{Con}_S,
\qquad S\vdash\operatorname{Con}_A\leftrightarrow\neg\Box_S\operatorname{Con}_S.
$$

From the preceding proof, $S\vdash\Box_SG\to\Box_S\bot$. Necessitating the equivalence between $G$ and $\operatorname{Con}_S$ and using [distribution](../../../../../normal-modal-distribution-axiom.md) therefore gives $S\vdash\Box_S\operatorname{Con}_S\to\Box_S\bot$. Its contrapositive is

$$
\boxed{S\vdash\operatorname{Con}_S\to\operatorname{Con}_{S+\neg\operatorname{Con}_S}.}
$$

This is an internal conditional statement. It does not assert that $S$ proves its own [consistency](../../../../../consistent-first-order-theory.md) or permits the [consistency](../../../../../consistent-first-order-theory.md) premise to be discarded.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
