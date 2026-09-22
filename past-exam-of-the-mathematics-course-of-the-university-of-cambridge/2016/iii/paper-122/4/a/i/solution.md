<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an object $X$ of a [braided monoidal category](../../../../../../../braided-monoidal-category.md), take its self-[braiding](../../../../../../../braiding.md)

$$
\boxed{y=c_{X,X}:X\otimes X\longrightarrow X\otimes X.}
$$

It is invertible by definition. Suppress canonical [associators](../../../../../../../associator.md) using the [monoidal coherence theorem](../../../../../../../monoidal-coherence-theorem.md), and put $R_{12}=y\otimes1$, $R_{23}=1\otimes y$. The hexagon identity gives

$$
c_{X,X\otimes X}=R_{23}R_{12}.
$$

Apply [naturality](../../../../../../../naturality.md) of this [braiding](../../../../../../../braiding.md) to the morphism $y:X\otimes X\to X\otimes X$ in its second argument. It says

$$
c_{X,X\otimes X}(1\otimes y)=(y\otimes1)c_{X,X\otimes X}.
$$

Substitution gives

$$
\boxed{R_{23}R_{12}R_{23}=R_{12}R_{23}R_{12}.}
$$

This is the equation for a [Yang–Baxter operator](../../../../../../../yang-baxter-operator.md). Restoring the uniquely determined [associators](../../../../../../../associator.md) gives the non-strict diagram in the paper. **Every object therefore has the canonical Yang–Baxter operator supplied by its self-braiding.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 122](../../../../paper-122-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
