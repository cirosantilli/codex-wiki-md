<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Prepare an ancillary [qubit](../../../../../../qubit.md) in

$$
|-\rangle=\frac{|0\rangle-|1\rangle}{\sqrt2},\qquad X|-\rangle=-|-\rangle.
$$

It can be prepared from $|0\rangle$ by an $X$ operation followed by a [Hadamard gate](../../../../../../hadamard-gate.md), independently of $g$. One call to the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) then gives [quantum phase kickback](../../../../../../phase-kickback.md):

$$
U_g|x\rangle|-\rangle=(-1)^{g(x)}|x\rangle|-\rangle.
$$

The data state receives a minus sign precisely on the basis vectors spanning $\mathcal G$, while the ancilla remains unchanged and unentangled. **One oracle call realizes the reflection**. By linearity it is the [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md)

$$
\boxed{I_{\mathcal G}=\sum_x(-1)^{g(x)}|x\rangle\langle x|=I-2\Pi_{\mathcal G}}
$$

with one oracle call. The ancillary preparation and its optional inverse use only fixed operations, so no additional knowledge of $g$ is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
