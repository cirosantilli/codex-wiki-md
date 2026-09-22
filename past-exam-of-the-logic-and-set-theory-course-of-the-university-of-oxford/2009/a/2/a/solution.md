<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With [generalization](../../../../../universal-generalization-rule.md) restricted to variables not free in open assumptions, the deduction theorem states

$$
\boxed{\Gamma\cup\{\alpha\}\vdash\beta\quad\Longleftrightarrow\quad\Gamma\vdash\alpha\to\beta.}
$$

The reverse direction follows by thinning and [modus ponens](../../../../../implication-elimination-rule.md). For the forward direction, induct on a derivation, keeping track of its actual assumption contexts. Axioms and assumptions already in $\Gamma$ yield $\alpha\to\chi$ by A1; the distinguished assumption $\alpha$ yields the permitted theorem $\alpha\to\alpha$. If a line $\chi$ is obtained by [modus ponens](../../../../../implication-elimination-rule.md) from $\eta$ and $\eta\to\chi$, the induction hypotheses and A2 derive $\alpha\to\chi$.

If a [generalization](../../../../../universal-generalization-rule.md) step depends on the discharged assumption, its variable $x$ is not free in $\alpha$ or the other open assumptions. Generalize the induction conclusion $\alpha\to\eta$ to $\forall x(\alpha\to\eta)$ and use A5 to derive $\alpha\to\forall x\eta$. If the subderivation does not depend on $\alpha$, its generalized conclusion can instead be retained as an independent derivation and A1 applied afterwards. Thinning merely enlarges the remaining context and preserves the induction claim. These cases are why assumption dependence, rather than a careless unrestricted universal rule, is essential.

In a presentation allowing [generalization](../../../../../universal-generalization-rule.md) freely from hypotheses, the corresponding theorem must instead explicitly require that no variable free in $\alpha$ is generalized in an $\alpha$-dependent line. Without that restriction $P(x)\vdash\forall xP(x)$ would incorrectly yield $\vdash P(x)\to\forall xP(x)$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
