# Noninjective linear measurement

↑ **Parent:** [Kernel of a linear map](kernel-of-a-linear-map-split.md)

When a measurement model is a [linear map](linear-map.md) $T$, its [kernel](kernel-of-a-linear-map-split.md) records changes that its readout cannot distinguish. For example, the [rectangular kernel and solution-fibre example](rectangular-kernel-and-solution-fibre-example.md) measures only $x+2y$ and $y+z$. Even exact readouts $(3,2)$ leave the whole [fiber](fiber-of-a-function.md) $u_0+\ker A$ possible. Repeating either readout with greater precision cannot distinguish those inputs: their outputs agree exactly. This ambiguity follows from a nontrivial [kernel](kernel-of-a-linear-map-split.md), rather than from measurement error.

Additional information can remove a [null direction of a linear map](null-direction-of-a-linear-map.md). In that example, adding a third [linear functional](linear-functional.md) that reads $y$ distinguishes $u_0+tv$, because its third readout is $t$. More generally, additional [linear functionals](linear-functional.md) $c_1,\ldots,c_k$ give unique recovery of all inputs exactly when

$$
\ker T\cap\ker c_1\cap\cdots\cap\ker c_k=\{0\}.
$$

This follows by applying the [trivial kernel](trivial-kernel.md) criterion to the combined [linear map](linear-map.md) $x\mapsto(Tx,c_1(x),\ldots,c_k(x))$. Merely adding repeated [linear equations](linear-equation.md) does not meet this condition. On a finite-dimensional input [vector space](vector-space-split.md), each added [scalar](scalar.md) readout can increase the [matrix rank](matrix-rank.md) by at most one, so at least $\dim\ker T$ extra independent readouts are needed for recovery of unrestricted inputs.

Restrictions on the possible inputs can also make recovery unique. If the allowed inputs form a [set](set-split.md) $D$, two allowed inputs are indistinguishable exactly when their difference is in the [kernel](kernel-of-a-linear-map-split.md). Thus $T$ is [injective](injective-function.md) on $D$ precisely when no difference of distinct points of $D$ is a [kernel](kernel-of-a-linear-map-split.md) [vector](vector.md). Such a restriction is extra information about the input; the original readout alone determines only its [fiber](fiber-of-a-function.md).

## ↑ Ancestors (6)

1. [Kernel of a linear map](kernel-of-a-linear-map-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
