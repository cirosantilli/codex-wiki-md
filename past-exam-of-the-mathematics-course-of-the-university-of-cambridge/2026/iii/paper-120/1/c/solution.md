<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On equivalence classes define

$$
[w]\preceq[v]iff\operatorname{Th}_\varphi(w)\subseteq\operatorname{Th}_\varphi(v),
$$

and, for every atomic proposition $p\in\Phi$, put $[w]\Vdash p$ exactly when $w\Vdash p$. This is well-defined, is a partial order, and makes atomic forcing persistent.

The [filtration of a Kripke model](../../../../../../filtration-of-a-kripke-model.md) truth lemma states

$$
[w]\Vdash\psi\iff w\Vdash\psi\qquad(\psi\in\Phi).
$$

Conjunction and disjunction are immediate by induction. For implication, if $w\Vdash\alpha\to\beta$ and $[w]\preceq[v]$, then $\alpha\to\beta$ belongs to $\operatorname{Th}_\varphi(v)$; if $[v]\Vdash\alpha$, induction gives $v\Vdash\alpha$, hence $v\Vdash\beta$ and $[v]\Vdash\beta$. Conversely, if $w\nVdash\alpha\to\beta$, some actual $v\geq w$ forces $\alpha$ but not $\beta$; persistence gives $[w]\preceq[v]$, which witnesses failure in the quotient. Thus every formula in $\Phi$ is preserved.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
