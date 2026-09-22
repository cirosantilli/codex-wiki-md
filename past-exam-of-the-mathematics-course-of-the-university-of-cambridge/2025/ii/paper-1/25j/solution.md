<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

A rational map $X\dashrightarrow Y$ between irreducible projective varieties is an equivalence class of morphisms from nonempty open subsets of $X$ to $Y$, with representatives identified when they agree on a nonempty open subset. It is regular at $p$ if some representative is defined on a neighborhood of $p$.

For

$$
\phi(x:y:z)=(xy:xz:z^2),
$$

the coordinates vanish together exactly at $(0:1:0)$ and $(1:0:0)$. Near the first point, the paths $z=0$ and $x=0$ have limiting images $(1:0:0)$ and $(0:0:1)$; near the second, the paths $z=0$ and $y=0$ have limiting images $(1:0:0)$ and $(0:1:0)$. No continuous extension exists there. Elsewhere the coordinates do not vanish together, so the map is regular.

Define

$$
\psi(u:v:w)=(v^2:uw:vw).
$$

Where all coordinates are nonzero,

$$
\psi\phi(x:y:z)=(x^2z^2:xyz^2:xz^3)=(x:y:z),
$$

and similarly $\phi\psi$ is the identity. Thus $\phi$ is birational and is an isomorphism on $\mathbb P^2\setminus Z(xyz)$.

For irreducibility of $P=x^2z^4-x^3y^3+z^6$, dehomogenize at $z=1$. Over $k(x)$ this is, up to a unit,

$$
y^3-\frac{x^2+1}{x^3}.
$$

The rational [function](../../../../../function-split.md) on the right is not a cube, since its valuation at either root of $x^2+1$ is one. The cubic is therefore irreducible over $k(x)$; Gauss's lemma gives irreducibility in $k[x,y]$. Since $z$ does not divide $P$, homogenization preserves irreducibility.

Writing $(u:v:w)=(xy:xz:z^2)$ transforms the equation into

$$
C:\quad v^2w-u^3+w^3=0.
$$

Its [partial derivatives](../../../../../partial-derivative.md) are $-3u^2$, $2vw$, and $v^2+3w^2$ up to common signs. Simultaneous vanishing forces $u=v=w=0$, impossible projectively, so $C$ is nonsingular. The inverse $\psi$ restricts on dense open subsets, proving that $V$ and $C$ are birational.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
