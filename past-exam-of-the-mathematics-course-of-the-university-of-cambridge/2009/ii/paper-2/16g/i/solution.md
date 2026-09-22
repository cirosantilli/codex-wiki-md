<h1 id="16g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

One Hilbert axiomatization of [classical propositional logic](../../../../../../classical-propositional-logic.md) uses the schemas $A\to(B\to A)$, $[A\to(B\to C)]\to[(A\to B)\to(A\to C)]$ and $(\neg B\to\neg A)\to(A\to B)$, with modus ponens as its inference rule. Other connectives can be defined from implication and negation. Syntactic entailment $\Gamma\vdash A$ means that a finite formal proof derives $A$ from the schemas and members of $\Gamma$. Consistency means that no formula and its negation are both derivable, equivalently no contradiction is derivable.

Use the standard deduction theorem, closure of derivability under modus ponens, and the maximal-consistency properties: a maximal consistent set contains exactly one of $A,\neg A$, is closed under derivability, and satisfies $A\to B\in\Phi$ exactly when $A\notin\Phi$ or $B\in\Phi$. These follow from the deduction theorem and the classical schemas; in particular adjoining a missing formula to a maximal set must yield a contradiction. Define $v(p)=T$ iff $p\in\Phi$. Induction on formula construction now proves

$$
v(A)=T\quad\Longleftrightarrow\quad A\in\Phi.
$$

For negation use the exactly-one property, and for implication use its displayed membership rule, which is precisely the Boolean truth table. Thus **every member of $\Phi$ is true under $v$**, providing the required valuation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [16G](../../16g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
