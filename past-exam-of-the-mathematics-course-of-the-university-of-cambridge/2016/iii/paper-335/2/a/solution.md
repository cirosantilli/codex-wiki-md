<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the time convention $e^{-i\omega t}$ and the outgoing [Sommerfeld radiation condition](../../../../../../sommerfeld-radiation-condition.md). Define the [outgoing Green function for the three-dimensional Helmholtz equation](../../../../../../outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md) by

$$
G_k(\mathbf r,\mathbf r')=\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|},\qquad
(\Delta_{\mathbf r}+k^2)G_k=-\delta(\mathbf r-\mathbf r').
$$

Away from $\mathbf r'$ it solves the homogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md). Integrating its radial derivative over a small sphere gives $-1$ in the zero-radius limit, verifying the sign of the [Dirac delta distribution](../../../../../../dirac-delta-function.md). At infinity it satisfies $(\partial_R-ik)G_k=o(R^{-1})$.

**For the positive source on the right-hand side, the outgoing field is**

$$
\boxed{\psi(\mathbf r,k)=-\int_A
\frac{e^{ik|\mathbf r-\mathbf r'|}}{4\pi|\mathbf r-\mathbf r'|}
Q(\mathbf r')\,d^3\mathbf r'.}
$$

Applying the [Helmholtz equation](../../../../../../helmholtz-equation.md) operator under this source representation gives $Q$. The minus sign is essential with the displayed [Green function](../../../../../../green-s-function.md) convention; defining the [Green function](../../../../../../green-s-function.md) to satisfy $LG=+\delta$ instead would absorb it. Here $A$ is the solid ball of radius $r_0$, as required by the volume source equation. Its finite volume and $Q\in L^2(A)$ make $Q$ integrable. The [Sommerfeld radiation condition](../../../../../../sommerfeld-radiation-condition.md) specifies the outgoing solution; without it one could add a homogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md) solution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
