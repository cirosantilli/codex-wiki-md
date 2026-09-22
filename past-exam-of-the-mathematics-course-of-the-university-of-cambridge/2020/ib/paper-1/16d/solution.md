<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

The [electric potential](../../../../../electric-potential.md) of a [point charge](../../../../../point-charge.md) $Q$ at the origin is

$$
\boxed{\Phi(\mathbf x)=\frac{Q}{4\pi\epsilon_0|\mathbf x|}}.
$$

For the two charges forming the dipole,

$$
\Phi(\mathbf x)=\frac{Q}{4\pi\epsilon_0}
\left(\frac1{|\mathbf x|}-\frac1{|\mathbf x+\mathbf d|}\right).
$$

The first-order [Taylor expansion](../../../../../taylor-expansion.md) at large $|\mathbf x|$ is

$$
\frac1{|\mathbf x+\mathbf d|}
=\frac1r-\frac{\mathbf d\cdot\mathbf x}{r^3}
+O\!\left(\frac{|\mathbf d|^2}{r^3}\right),
$$

and therefore, with the [electric dipole moment](../../../../../electric-dipole-moment.md) $\mathbf p=Q\mathbf d$,

$$
\boxed{\Phi(\mathbf x)=\frac1{4\pi\epsilon_0}
\frac{\mathbf p\cdot\mathbf x}{r^3}}
$$

to leading order. Taking the interaction of a second dipole with the corresponding [electric field](../../../../../electric-field.md) gives the stated [electric dipole-dipole interaction](../../../../../electric-dipole-dipole-interaction.md)

$$
U=\frac1{8\pi\epsilon_0}
\left(\frac{\mathbf p_1\cdot\mathbf p_2}{r^3}
-\frac{3(\mathbf p_1\cdot\mathbf r)(\mathbf p_2\cdot\mathbf r)}{r^5}\right).
$$

Let the lattice spacing be $d$ and write the central dipole as

$$
\mathbf p=p(\cos\theta,\sin\theta).
$$

Its two horizontal neighbours have moment $p(\cos\theta,-\sin\theta)$. For either one, the expression in parentheses, after extracting $d^{-3}$, is

$$
-p^2(1+\cos^2\theta).
$$

Its two vertical neighbours have moment $p(-\cos\theta,\sin\theta)$, and each contributes instead

$$
-p^2(1+\sin^2\theta).
$$

Adding all four nearest-neighbour interactions and using the [Pythagorean trigonometric identity](../../../../../pythagorean-trigonometric-identity.md) gives

$$
\boxed{U_{\mathrm{nearest}}
=-\frac{6p^2}{8\pi\epsilon_0d^3}
=-\frac{3p^2}{4\pi\epsilon_0d^3}}.
$$

The angle has cancelled, so the energy is independent of $\theta$.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
