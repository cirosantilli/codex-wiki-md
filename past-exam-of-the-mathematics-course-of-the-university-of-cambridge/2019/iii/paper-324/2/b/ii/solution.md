<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Applying the two [modular-addition quantum oracles](../../../../../../../modular-addition-quantum-oracle.md) consecutively adds $h(x)+r(x)=0\pmod M$ to the answer register. Thus

$$
\boxed{U_r=U_h^{-1}.}
$$

Let $S_M|y\rangle=|-y\pmod M\rangle$. Applying $I\otimes S_M$, then $U_h$, then $I\otimes S_M$ gives

$$
|x,y\rangle\longmapsto|x,-y\rangle
\longmapsto|x,-y+h(x)\rangle
\longmapsto|x,y-h(x)\rangle.
$$

Therefore

$$
\boxed{U_h^{-1}=(I\otimes S_M)U_h(I\otimes S_M),}
$$

using one query and two [unitary operators](../../../../../../../unitary-operator.md) independent of $h$. This is [modular-oracle inversion by negation](../../../../../../../modular-oracle-inversion-by-negation.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
