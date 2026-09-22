<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $\mathbf B=0$, part (b) gives $\mathbf V=2\mathbf A/3$ and $\boldsymbol\omega=0$. The total boundary velocity is therefore

$$
\mathbf V+\mathbf u_s
=-\frac13\mathbf A+\frac{\mathbf x(\mathbf A\mathbin\cdot\mathbf x)}{a^2}.
$$

The decaying [velocity potential](../../../../../../velocity-potential.md)

$$
\phi=-\frac{a^3}{3}\frac{\mathbf A\mathbin\cdot\mathbf x}{r^3}
$$

is harmonic for $r>a$, and

$$
\boxed{\mathbf u=\nabla\phi
=-\frac{a^3}{3}\nabla\left(\frac{\mathbf A\mathbin\cdot\mathbf x}{r^3}\right)}
$$

has exactly this value at $r=a$. It is a force-free potential-dipole field and decays as $r^{-3}$.

When $\mathbf A=0$, define the degree-three [harmonic polynomial](../../../../../../harmonic-polynomial.md)

$$
H_3(\mathbf x)=(\mathbf B\mathbin\cdot\mathbf x)^3
-\frac35|\mathbf B|^2r^2(\mathbf B\mathbin\cdot\mathbf x).
$$

An appropriate decaying harmonic potential is

$$
\Psi=C\frac{H_3(\mathbf x)}{r^7},
\qquad
\mathbf u=\nabla\Psi\times\mathbf x.
$$

Indeed, the tangential boundary value is proportional to

$$
\left[\frac{(\mathbf B\mathbin\cdot\mathbf x)^2}{a^3}
-\frac{|\mathbf B|^2}{5a}\right]\mathbf B\times\mathbf x,
$$

which combines the prescribed slip with the rigid rotation found in part (b). Since $H_3/r^7=O(r^{-4})$ and multiplication of its gradient by $\mathbf x$ preserves that order, the exterior velocity decays as

$$
\boxed{|\mathbf u|=O(r^{-4}).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
