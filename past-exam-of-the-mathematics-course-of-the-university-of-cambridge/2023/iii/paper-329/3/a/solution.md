<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $x$ downslope, $y$ across the slope, and $z$ normal to the plane. The leading normal momentum balance gives

$$
p=p_a+\rho g\cos\alpha\,(h-z).
$$

The tangential [lubrication theory](../../../../../../lubrication-theory.md) equations, with no slip at $z=0$ and zero tangential stress at $z=h$, then give the depth-integrated flux

$$
\mathbf q=\frac{\rho gh^3}{3\mu}
\left(\sin\alpha\,\mathbf e_x-cos\alpha\,\nabla h\right).
$$

For $\alpha\ll1$, define

$$
\widetilde h=\frac h{h_0},
\qquad
(\widetilde x,\widetilde y)
=\frac\alpha{h_0}(x,y),
\qquad
\widetilde{\mathbf q}
=\frac{3\mu}{\rho g\alpha h_0^3}\mathbf q.
$$

Dropping tildes, steady [mass conservation](../../../../../../mass-conservation.md) $\nabla\mathbin\cdot\mathbf q=0$ becomes

$$
\boxed{\nabla\mathbin\cdot(h^3\mathbf e_x)
=\nabla\mathbin\cdot(h^3\nabla h)},
$$

with $h\to1$ as $x\to-\infty$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
