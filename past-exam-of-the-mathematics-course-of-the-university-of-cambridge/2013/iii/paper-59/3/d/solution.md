<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The class [NC1](../../../../../../nc1.md) consists of languages having polynomial-size, bounded-fan-in [Boolean circuit](../../../../../../boolean-circuit.md) families of depth $O(\log n)$. Under a uniform convention one requires the wiring to be constructible in [logarithmic space](../../../../../../logarithmic-space.md); the construction below meets that requirement as well as the nonuniform one.

Write a length-$n$ binary input with most significant bit first as $x_1\cdots x_n$. Since $2^m\equiv(-1)^m\pmod3$,

$$
x\equiv\sum_{i=1}^n(-1)^{n-i}x_i\pmod3.
$$

Represent residues zero, one and two by two bits, respectively $00,01,10$. Each input produces residue zero when it is zero; when it is one it produces residue one or two according to the parity of $n-i$. This uses only constants and wires.

A two-residue addition modulo three is a fixed function of four [Boolean variables](../../../../../../boolean-variable.md) and has a constant-size, constant-depth bounded-fan-in [Boolean circuit](../../../../../../boolean-circuit.md). Define its unused $11$ encodings arbitrarily; valid inputs always produce a valid residue encoding. Use a balanced binary tree of these adders, padding with zero residues to a power of two. There are $O(n)$ adders and $O(\log n)$ layers. A final constant-size gate checks that the residue is $00$.

This [balanced finite-monoid reduction circuit](../../../../../../balanced-finite-monoid-reduction-circuit.md) is uniform: leaf signs follow index parity and internal connections follow the indices in the balanced tree, all calculable in [logarithmic space](../../../../../../logarithmic-space.md). Leading zeros cause no difficulty; the empty input can be assigned the zero-integer constant convention. Consequently

$$
\boxed{\mathrm{MOD3}\in\mathrm{NC}^1}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
