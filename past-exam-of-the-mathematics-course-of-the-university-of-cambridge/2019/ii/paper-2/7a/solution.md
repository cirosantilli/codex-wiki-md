<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Apply the [residue theorem](../../../../../residue-theorem.md) to the upper-half-plane semicircle, with a small semicircular indentation above the pole at $z=0$. The large arc contributes zero because $f(z)/z\to0$, so

$$
\frac{f(z)}{z(z^2+a^2)}=o(|z|^{-2}).
$$

The small indentation is traversed clockwise and contributes $-i\pi$ times the [residue](../../../../../residue.md) at zero. The only pole strictly inside the indented contour is $z=ia$. Therefore

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{f(x)}{x(x^2+a^2)}\,dx
=2\pi i\operatorname{Res}_{z=ia}\frac{f(z)}{z(z^2+a^2)}
+i\pi\operatorname{Res}_{z=0}\frac{f(z)}{z(z^2+a^2)}.
$$

The two residues are

$$
\operatorname{Res}_{z=ia}=-\frac{f(ia)}{2a^2},
\qquad
\operatorname{Res}_{z=0}=\frac{f(0)}{a^2}.
$$

Consequently the [Cauchy principal value](../../../../../cauchy-principal-value.md) is

$$
\boxed{\operatorname{PV}\int_{-\infty}^{\infty}\frac{f(x)}{x(x^2+a^2)}\,dx
=\frac{i\pi}{a^2}\bigl(f(0)-f(ia)\bigr).}
$$

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
