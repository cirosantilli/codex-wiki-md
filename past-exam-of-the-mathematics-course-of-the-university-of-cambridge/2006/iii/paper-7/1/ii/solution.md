<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the given integer $u$ satisfying $u^2\equiv-1\pmod p$. The [Euclidean lattice](../../../../../../euclidean-lattice.md) under consideration has basis $(1,u),(0,p)$, because every vector in it is uniquely $(a,ua+bp)$ with $a,b\in\mathbb Z$. Its fundamental parallelogram therefore has area

$$
\left|\det\begin{pmatrix}1&0\\u&p\end{pmatrix}\right|=p.
$$

We use the following two-dimensional form of the [Minkowski convex body theorem](../../../../../../minkowski-s-theorem.md): a convex, centrally symmetric measurable subset of $\mathbb R^2$ of area strictly greater than four times the covolume of a full-rank [Euclidean lattice](../../../../../../euclidean-lattice.md) contains a nonzero vector of that lattice. Apply it to the closed disk of squared radius $3p/2$. Its area is $3\pi p/2>4p$, so it contains a nonzero lattice vector $(a,b)$ satisfying

$$
0<a^2+b^2\leq\frac{3p}{2}<2p.
$$

On the other hand the defining [modular congruence](../../../../../../modular-congruence.md) and $u^2\equiv-1\pmod p$ imply

$$
a^2+b^2\equiv a^2+(ua)^2=(1+u^2)a^2\equiv0\pmod p.
$$

There is exactly one positive multiple of $p$ strictly below $2p$, so $\boxed{p=a^2+b^2}$. Neither coordinate can be zero, since a prime is not the square of an integer. This [congruence lattice proof of the prime sum of two squares](../../../../../../congruence-lattice-proof-of-the-prime-sum-of-two-squares.md) proves the required case of the [sum of two squares theorem](../../../../../../sum-of-two-squares-theorem.md) without assuming any conclusion at the critical area $4p$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
