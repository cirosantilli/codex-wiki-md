<h1 id="26h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [smooth function](../../../../../../smooth-function.md)

$$
F:\mathbb R^{n+1}\longrightarrow\mathbb R,
\qquad
F(x)=\lVert x\rVert^2.
$$

At $x\in F^{-1}(1)$ its derivative is

$$
D_xF(v)=2x\mathbin\cdot v.
$$

This linear map is surjective because $x\ne0$; for example, $D_xF(x)=2$. Hence one is a [regular value](../../../../../../regular-value.md), and the [regular level set theorem](../../../../../../regular-level-set-theorem.md) makes

$$
S^n=F^{-1}(1)
$$

an embedded codimension-one submanifold of $\mathbb R^{n+1}$. Its tangent space is the kernel of the derivative:

$$
\boxed{T_xS^n
=\ker D_xF
=\{v:x\mathbin\cdot v=0\}
=x^\perp}.
$$

This is the [unit sphere as a regular level set](../../../../../../unit-sphere-as-a-regular-level-set.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26H](../../26h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
