<h1 id="1/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [chain rule](../../../../../../../chain-rule.md) yields

$$
\{F\circ f,G\circ f\}_{q,p}
=(\nabla F\circ f)^T AJA^T(\nabla G\circ f).
$$

If $f$ is a [canonical transformation](../../../../../../../canonical-transformation.md), the [symplectic matrix](../../../../../../../symplectic-matrix.md) identity $AJA^T=J$ makes this expression $\{F,G\}_{Q,P}\circ f$. Thus preservation of the [symplectic form](../../../../../../../symplectic-form.md) implies preservation of every [Poisson bracket](../../../../../../../poisson-bracket.md), for all $C^1$ functions.

Conversely, assume this [Poisson bracket](../../../../../../../poisson-bracket.md) identity for every $F,G$. Take $F(Z)=u\cdot Z$ and $G(Z)=v\cdot Z$, for arbitrary constant [vectors](../../../../../../../vector.md) $u,v\in\mathbb R^{2n}$. It gives $u^TAJA^Tv=u^TJv$. Since this holds for every $u,v$, $AJA^T=J$, hence $A^TJA=J$. Therefore **preservation of all [Poisson brackets](../../../../../../../poisson-bracket.md) is equivalent to canonicity**. Only first [derivatives](../../../../../../../derivative.md) of $f,F,G$ enter this argument.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [1](../../../1.md)
4. [Paper 20](../../../../paper-20-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
