<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The answer is **no** with the integer-translation and dilation conventions of this [multiresolution analysis](../../../../../../multiresolution-analysis.md). The [orthonormal basis](../../../../../../orthonormal-basis.md) axiom forces $V_0$ to consist of $L^2$ functions constant on the cells $[k-1/2,k+1/2)$. Dilation forces $V_1$ to consist of functions constant on $[k/2-1/4,k/2+1/4)$. However, the proposed [scaling function](../../../../../../scaling-function.md) changes value at $1/2$, in the interior of the $V_1$ cell $[1/4,3/4)$. It is therefore not in $V_1$, contradicting nesting:

$$
\boxed{V_0\not\subset V_1.}
$$

Changing values at endpoints makes no difference in $L^2$. The usual [Haar wavelet](../../../../../../haar-wavelet.md) instead uses the [scaling function](../../../../../../scaling-function.md) $\chi_{[0,1)}$; an arbitrary half-unit translation does not preserve the required refinement grid.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
