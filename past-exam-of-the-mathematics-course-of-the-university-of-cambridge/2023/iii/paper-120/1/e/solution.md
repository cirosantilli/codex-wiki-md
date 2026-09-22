<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose neither $\phi$ nor $\psi$ is provable. By the [Kripke completeness theorem for intuitionistic propositional logic](../../../../../../kripke-completeness-theorem-for-intuitionistic-propositional-logic.md), there are rooted [Kripke countermodels](../../../../../../kripke-countermodel.md) with roots $r_\phi\nVdash\phi$ and $r_\psi\nVdash\psi$. Take their disjoint union and place a fresh world $r$ below every world in both components, forcing no propositional variables at $r$ beyond those required by persistence.

If $r\Vdash\phi$, persistence would imply $r_\phi\Vdash\phi$, a contradiction; similarly $r\nVdash\psi$. Thus $r\nVdash\phi\vee\psi$. By soundness, $\phi\vee\psi$ is not provable. Taking the contrapositive proves the [disjunction property of intuitionistic propositional logic](../../../../../../disjunction-property-of-intuitionistic-propositional-logic.md):

$$
\boxed{\vdash_{\mathrm{IPC}}\phi\vee\psi
\quad\Longrightarrow\quad
\vdash_{\mathrm{IPC}}\phi\ \text{or}\ \vdash_{\mathrm{IPC}}\psi.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
