<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [adjoint functor theorem for complete lattices](../../../../../../adjoint-functor-theorem-for-complete-lattices.md) says that a monotone map $f:A\to B$ between complete lattices preserves arbitrary joins exactly when it has a right adjoint

$$
f^*(b)=\bigvee\{a:f(a)\leq b\}.
$$

A right adjoint preserves arbitrary meets. Regard it as the join-preserving map

$$
f^*:B^{\mathrm{op}}\longrightarrow A^{\mathrm{op}}.
$$

Thus define $A^*=A^{\mathrm{op}}$ and send $f$ to its right adjoint. Since a left adjoint is the right adjoint of its right adjoint after reversing orders, $(f^*)^*=f$ and $(A^*)^*=A$. This gives the involutive self-duality

$$
\boxed{(-)^*:\mathbf{CSLat}^{\mathrm{op}}\longrightarrow\mathbf{CSLat}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
