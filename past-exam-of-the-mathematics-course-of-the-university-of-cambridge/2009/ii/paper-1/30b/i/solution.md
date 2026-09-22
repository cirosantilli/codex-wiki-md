<h1 id="30b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $z=(x,v)$ and $B(z)=(v,-\nabla V(x))$. The [characteristic flow map](../../../../../../characteristic-flow-map.md) $\Phi_t$ solves $\dot z=B(z)$. Its vector field is globally [Lipschitz continuous](../../../../../../lipschitz-continuity.md), so [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md) gives a unique global flow with inverse $\Phi_{-t}$. Also $\operatorname{div}_z B=0$.

The proposed [Dirac measure](../../../../../../dirac-measure.md) is the unit mass at $\Phi_t(z_0)$. For every compactly supported smooth test function $\psi$,

$$
\frac d{dt}\langle f_t,\psi\rangle=\frac d{dt}\psi(\Phi_t(z_0))
=B(\Phi_t(z_0))\cdot\nabla\psi(\Phi_t(z_0))=\langle f_t,B\cdot\nabla\psi\rangle.
$$

This is the [weak formulation](../../../../../../weak-formulation.md) of $f_t+\operatorname{div}(Bf)=0$, equal to the [Liouville equation](../../../../../../liouville-equation.md) because $\operatorname{div}B=0$. The initial unit mass is recovered at $t=0$. The characteristic equations are precisely $\dot{\widehat x}=\widehat v$, $\dot{\widehat v}=-\nabla V(\widehat x)$; the time-derivative dots, lost in the converted text, are present in the PDF.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [30B](../../30b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
