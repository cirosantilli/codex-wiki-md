<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If zero is admitted as a limit case, the assertion there is immediate since $\gamma_0=0$. For a nonzero limit, let $\kappa=|\lambda|$, an infinite [initial ordinal](../../../../../initial-ordinal.md). There are two cases; separating them avoids choosing an entire family of [bijections](../../../../../bijection.md) at earlier stages.

If $\kappa<\lambda$, the hypothesis applies at $\kappa$. Part (a) gives a [bijection](../../../../../bijection.md) $g_\kappa:\kappa^2\to\gamma_\kappa$, whose range has [cardinality](../../../../../cardinality.md) $\kappa$ by hypothesis. Fix one [bijection](../../../../../bijection.md) $\lambda\to\kappa$; taking its product gives $\lambda^2\cong\kappa^2$. Since $g_\lambda$ is also bijective onto its range, these maps give $\boxed{|\gamma_\lambda|=\kappa=|\lambda|}$.

If $\lambda=\kappa$ is itself an [initial ordinal](../../../../../initial-ordinal.md), suppose $\gamma_\lambda>\kappa$. Continuity gives $\gamma_\lambda=\bigcup_{\alpha<\kappa}\gamma_\alpha$, so some earlier $\gamma_\alpha$ contains the [ordinal](../../../../../ordinal-split.md) $\kappa$. If $\alpha$ is finite then $\gamma_\alpha=\alpha^2$ is finite, impossible. If $\alpha$ is infinite, the hypothesis gives $|\gamma_\alpha|=|\alpha|<\kappa$, again impossible because its [ordinal](../../../../../ordinal-split.md) range contains an initial segment of size $\kappa$.

Thus $\gamma_\lambda\leq\kappa$. Conversely, [transfinite induction](../../../../../transfinite-induction.md) gives $\gamma_\alpha\geq\alpha$: each successor appends a nonempty row and limits take unions. In particular $\gamma_\lambda\geq\lambda=\kappa$. Hence $\gamma_\lambda=\kappa$ in this case, proving the required cardinal equality as well. The argument includes $\lambda=\omega$, whose earlier stages are finite.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
