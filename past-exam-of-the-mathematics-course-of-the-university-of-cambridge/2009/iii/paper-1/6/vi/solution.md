<h1 id="6/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

**False, even when the HNN extension also has a finite presentation.** Take the base $P=F_m\times F_m$ and its [Mihailova subgroup](../../../../../../mihailova-subgroup.md) $L$ from Question 4(b). Its [word problem for a group](../../../../../../word-problem-for-groups.md) is soluble: project a word to each free factor and freely reduce both projections, as in part (iv). The base is finitely presented, but the [HNN extension](../../../../../../hnn-extension.md)

$$
G=\langle P,t\mid t^{-1}\ell t=\ell\ (\ell\in L)\rangle
$$

has insoluble word problem by the explicit reduction in Question 4(b). Namely, for an input word $w$ in the presentation with insoluble word problem, set $p=(1,w)$; then

$$
\boxed{t^{-1}ptp^{-1}=1\text{ in }G\quad\Longleftrightarrow\quad p\in L
\quad\Longleftrightarrow\quad w=1\text{ in }H.}
$$

The obstruction is undecidable membership in the associated subgroup, not undecidable equality in the base. Soluble base word problem alone does not let one recognize the pinches needed for a [normal form theorem for an HNN extension](../../../../../../normal-form-theorem-for-an-hnn-extension.md) algorithm.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
