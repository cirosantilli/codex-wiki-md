<h1 id="a/1/e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First note that a substring which is itself a [logical formula](../../../../../../logical-formula.md) must coincide with a subtree of the [formula syntax tree](../../../../../../syntax-tree-of-a-formula.md) of the surrounding [logical formula](../../../../../../logical-formula.md). Indeed, a [logical formula](../../../../../../logical-formula.md) can begin only at a [logical variable](../../../../../../logical-variable.md), a [negation](../../../../../../negation.md) symbol or an opening parenthesis. Every such position in a valid [logical formula](../../../../../../logical-formula.md) is the start of one of its parsed subtrees. If $\beta$ is the [logical formula](../../../../../../logical-formula.md) at that subtree and $\alpha$ is another [logical formula](../../../../../../logical-formula.md) starting at the same position, one is an initial segment of the other; [prefix-freeness of fully parenthesized formulas](../../../../../../prefix-freeness-of-fully-parenthesized-formulas.md) from the preceding part forces $\alpha=\beta$.

Now consider a final [subformula](../../../../../../subformula.md). For a [logical variable](../../../../../../logical-variable.md), it can only be the whole [logical formula](../../../../../../logical-formula.md). For a binary [logical implication](../../../../../../logical-implication.md) $(\psi\to\chi)$, every proper subtree is contained in $\psi$ or $\chi$ and finishes before the final closing parenthesis of the whole expression. It therefore cannot be a final substring of the whole. The only remaining possible outer formation is [negation](../../../../../../negation.md). Thus

$$
\boxed{\alpha=\phi\quad\text{or}\quad\phi=\neg\psi\text{ for some formula }\psi.}
$$

The second alternative is a necessary possibility, not a claim that every negated [logical formula](../../../../../../logical-formula.md) has every one of its [subformulas](../../../../../../subformula.md) as a suffix.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
