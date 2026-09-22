<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Composition and inversion in the [Affine group of the complex line](../../../../../../affine-group-of-the-complex-line.md) are

$$
f_{a,b}\circ f_{a',b'}=f_{aa',\,ab'+b},
\qquad
f_{a,b}^{-1}=f_{a^{-1},\,-a^{-1}b}.
$$

The map

$$
\rho:G\longrightarrow\mathbb C^\times,\qquad
\rho(f_{a,b})=a
$$

is therefore a surjective [group homomorphism](../../../../../../group-homomorphism.md) with kernel

$$
N=\{f_{1,b}:b\in\mathbb C\}\cong(\mathbb C,+).
$$

Its target is [Abelian](../../../../../../abelian-group.md), so $[G,G]\subseteq N$. On the other hand, the stated computation gives

$$
[f_{a,1},f_{1,b}]=f_{1,b(1-a^{-1})}.
$$

Fixing any $a\ne1$ and varying $b$ produces every translation. Thus $N\subseteq[G,G]$, and hence

$$
\boxed{[G,G]=N\cong(\mathbb C,+),\qquad
G/[G,G]\cong\mathbb C^\times,\qquad
\pi(f_{a,b})=a.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
