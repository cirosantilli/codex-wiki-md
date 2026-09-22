<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [graph state](../../../../../../../graph-state.md) has computational-basis expansion

$$
|G\rangle=\frac1{2^{|V|/2}}
\sum_{x\in\{0,1\}^{|V|}}
(-1)^{\sum_{(r,s)\in E}x_rx_s}|x\rangle.
$$

For the path $G_A$ with edges $(1,2)$ and $(2,3)$,

$$
\boxed{
|G_A\rangle=\frac1{\sqrt8}(
|000\rangle+|001\rangle+|010\rangle-|011\rangle
+|100\rangle+|101\rangle-|110\rangle+|111\rangle)}.
$$

For the triangle $G_B$, the extra edge $(3,1)$ changes the phase whenever $x_1=x_3=1$, giving

$$
\boxed{
|G_B\rangle=\frac1{\sqrt8}(
|000\rangle+|001\rangle+|010\rangle-|011\rangle
+|100\rangle-|101\rangle-|110\rangle-|111\rangle)}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
