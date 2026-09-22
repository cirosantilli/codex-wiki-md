<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Run the perfect discriminator on the supplied state and record whether the result is $i=0$ or $i=1$. For each $i$, choose a unitary $V_i$ satisfying

$$
V_i|0\rangle=|\phi_i\rangle,
$$

which is possible by extending $|\phi_i\rangle$ to an orthonormal basis. Prepare two fresh systems in $|0\rangle|0\rangle$ and, controlled by the classical outcome $i$, apply $V_i\otimes V_i$. The output is

$$
|\phi_i\rangle|\phi_i\rangle.
$$

The discriminator may destroy its input; the two freshly prepared outputs still implement cloning on this known pair. This is the construction that [perfect discrimination implies cloning for a known state family](../../../../../../perfect-discrimination-implies-cloning-for-a-known-state-family.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
