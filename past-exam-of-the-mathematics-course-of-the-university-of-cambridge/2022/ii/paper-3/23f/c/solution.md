<h1 id="23f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\zeta=e^{2\pi i/n}$ and define Möbius transformations

$$
r(z)=\zeta z,
\qquad
s(z)=\frac1z.
$$

They satisfy

$$
r^n=s^2=1,
\qquad srs=r^{-1},
$$

and the $2n$ maps $r^k$ and $sr^k$ are distinct. They therefore give a faithful action of the [dihedral group](../../../../../../dihedral-group.md) $D_{2n}$ on the [Riemann sphere](../../../../../../riemann-sphere.md).

The [rational function](../../../../../../rational-function.md)

$$
\boxed{
f(z)=z^n+z^{-n}=\frac{z^{2n}+1}{z^n}
}
$$

is invariant under both $r$ and $s$, so it is constant on every orbit. Conversely, for nonzero finite $z_1,z_2$, put $u=z_1^n$ and $v=z_2^n$. Equality of the function values gives

$$
u+u^{-1}=v+v^{-1}
\quad\Longleftrightarrow\quad
(u-v)(uv-1)=0.
$$

If $u=v$, then $z_2=\zeta^kz_1=r^kz_1$ for some $k$. If $uv=1$, then $z_2=\zeta^k/z_1=r^ksz_1$ for some $k$. Finally, zero and infinity both map to infinity and are interchanged by $s$. Hence

$$
\boxed{f(z_1)=f(z_2)\quad\Longleftrightarrow\quad z_1,z_2\text{ lie in the same }D_{2n}\text{-orbit}}.
$$

This is the [orbit-separating invariant for the standard dihedral action on the Riemann sphere](../../../../../../orbit-separating-invariant-for-the-standard-dihedral-action-on-the-riemann-sphere.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23F](../../23f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
