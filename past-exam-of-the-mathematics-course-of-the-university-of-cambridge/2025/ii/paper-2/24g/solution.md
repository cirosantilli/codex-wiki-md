<h1 id="24g/solution">Solution</h1>

↑ **Parent:** [24G](../24g.md)

The identity theorem says that if two holomorphic functions on a connected Riemann surface agree on a set having an accumulation point, then they agree everywhere.

Apply local coordinates to their difference $F$. The power-series proof in the plane shows that near any point, either $F$ vanishes identically or its zeros are isolated: if the first nonzero Taylor coefficient has order $m$, then $F(z)=(z-z_0)^mG(z)$ with $G(z_0)\ne0$. An accumulation point of the zero set therefore has a neighbourhood on which $F=0$. The set of points having such a neighbourhood is nonempty and open. It is also closed: near a limit point, a coordinate neighbourhood contains an open set on which $F=0$, and the planar identity theorem makes $F$ vanish throughout that coordinate neighbourhood. Connectedness now makes this set the whole surface.

For a nonempty connected open set $U\subset\mathbb R^2$, a function $h:U\to\mathbb R$ is harmonic when $h\in C^2(U)$ and

$$
\Delta h=h_{xx}+h_{yy}=0.
$$

On a sufficiently small disc, the one-form

$$
-h_y\,dx+h_x\,dy
$$

is closed and hence equals $dk$ for some $k$. The Cauchy--Riemann equations then make $h+ik$ holomorphic. Holomorphic functions are smooth, so $h\in C^\infty(U)$.

A real-valued function $H$ on a Riemann surface is harmonic when, in every holomorphic chart $z$, its coordinate expression is harmonic. This definition is chart-independent. If $w=w(z)$ is a holomorphic transition map, the chain rule and Cauchy--Riemann equations give

$$
\Delta_z(H\circ w)=|w'(z)|^2(\Delta_w H)\circ w.
$$

**Thus vanishing of the Laplacian is preserved by every change of holomorphic coordinate.**

## ↑ Ancestors (10)

1. [24G](../24g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
