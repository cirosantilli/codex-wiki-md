<h1 id="24f/solution">Solution</h1>

↑ **Parent:** [24F](../24f.md)

Let $F:X\to Y$ be a nonconstant [holomorphic map](../../../../../holomorphic-map.md) of degree $d$ between compact connected Riemann surfaces. At $p\in X$, let $e_p$ be the [ramification index of a holomorphic map](../../../../../ramification-index-of-a-holomorphic-map.md). Choose a triangulation of $Y$ containing every branch value among its vertices, and lift it to $X$.

If the target triangulation has $V$ vertices, $E$ edges, and $T$ triangles, then the lifted triangulation has $dE$ edges and $dT$ triangles, because no branch value lies in an edge or face interior. For a target vertex $v$, local degree counting gives

$$
\sum_{p\in F^{-1}(v)}e_p=d.
$$

Consequently the number of vertices above $v$ is

$$
|F^{-1}(v)|
=d-\sum_{p\in F^{-1}(v)}(e_p-1).
$$

Writing $R=\sum_{p\in X}(e_p-1)$, the [Euler characteristic](../../../../../euler-characteristic.md) is therefore

$$
\chi(X)=(dV-R)-dE+dT=d\chi(Y)-R.
$$

Since a compact orientable surface of genus $g$ has Euler characteristic $2-2g$, this [Triangulation proof of the Riemann-Hurwitz formula](../../../../../triangulation-proof-of-the-riemann-hurwitz-formula.md) gives

$$
2-2g_X=d(2-2g_Y)-\sum_{p\in X}(e_p-1),
$$

or equivalently

$$
\boxed{2g_X-2=d(2g_Y-2)+\sum_{p\in X}(e_p-1)}.
$$

Now extend a cubic polynomial $f:\mathbb C\to\mathbb C$ to a degree-three holomorphic map

$$
F:\mathbb P^1(\mathbb C)\to\mathbb P^1(\mathbb C)
$$

of the [Riemann sphere](../../../../../riemann-sphere.md). Both genera are zero, so Riemann--Hurwitz gives

$$
\sum_p(e_p-1)=2\cdot3-2=4.
$$

The point at infinity is totally ramified with $e_\infty=3$, contributing two. Thus the finite points contribute exactly two. There are consequently two cases.

If there is one finite ramification point $\alpha$, it has index three. Choose an affine source map $h$ sending zero to $\alpha$. Then

$$
(f\circ h)'(z)=cz^2
$$

for some $c\ne0$, and integration gives

$$
f\circ h(z)=\frac c3z^3+d.
$$

An affine target map subtracts $d$ and rescales by $3/c$, yielding $z^3$.

Otherwise there are two distinct finite ramification points, each of index two. Choose an affine source map $h$ sending $-1$ and $1$ to them. The derivative of $f\circ h$ is then a nonzero multiple of $z^2-1$:

$$
(f\circ h)'(z)=c(z^2-1).
$$

Hence

$$
f\circ h(z)=c\left(\frac{z^3}{3}-z\right)+d.
$$

The affine target map $g(w)=(w-d)/c$ gives

$$
g\circ f\circ h(z)=\frac{z^3}{3}-z
=z\left(\frac{z^2}{3}-1\right).
$$

Therefore the [affine normal forms of a complex cubic polynomial](../../../../../affine-normal-forms-of-a-complex-cubic-polynomial.md) are precisely

$$
\boxed{z^3\quad\text{and}\quad z(z^2/3-1)}.
$$

## ↑ Ancestors (10)

1. [24F](../24f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
