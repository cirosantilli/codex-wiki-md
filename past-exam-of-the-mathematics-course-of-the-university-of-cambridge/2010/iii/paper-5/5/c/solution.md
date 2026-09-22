<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The local [Harnack inequality for harmonic functions](../../../../../../harnack-inequality-for-harmonic-functions.md) states that if $u\geq0$ is harmonic on a neighbourhood of $\overline{B_{4r}(a)}$, then

$$
\boxed{\sup_{B_r(a)}u\leq3^n\inf_{B_r(a)}u.}
$$

More generally, for any compact $K$ in a connected open domain $\Omega$, there is $C=C(K,\Omega,n)$ such that $\sup_Ku\leq C\inf_Ku$ for every nonnegative harmonic $u$ on $\Omega$. Positivity is essential; the assertion is not for arbitrary sign-changing functions.

First prove the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md). For a smooth harmonic function the spherical mean has derivative

$$
m_x'(t)=\frac1{|\mathbb S^{n-1}|t^{n-1}}\int_{B_t(x)}\Delta u=0,
$$

so it equals $u(x)$; integration in the radius gives the ball mean property. The preceding [Weyl lemma](../../../../../../weyl-lemma.md) supplies smoothness if harmonicity was initially distributional.

For $x,z\in B_r(a)$ the inclusion $B_r(x)\subset B_{3r}(z)\subset B_{4r}(a)$ and nonnegativity give

$$
u(x)=\frac1{|B_r|}\int_{B_r(x)}u\leq\frac1{|B_r|}\int_{B_{3r}(z)}u=3^nu(z).
$$

Taking the supremum over $x$ and the infimum over $z$ proves the local estimate directly. To obtain the compact-set form, connect centres of a finite ball cover of $K$ to a fixed interior point by paths in $\Omega$. The compact union of those paths stays a positive distance from the complement of $\Omega$. Subdivide the paths into finitely many steps small enough that the local estimate applies at consecutive points. Multiply the finitely many comparison constants, first from one point of $K$ to the reference point and then to any other point of $K$. This gives a constant independent of $u$. In particular a nonnegative harmonic function is either everywhere positive or identically zero on each connected component.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
