<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write an element of the [Integer Heisenberg group](../../../../../../integer-heisenberg-group.md) as $(x,y,z)$. [Matrix multiplication](../../../../../../matrix-multiplication.md) gives

$$
(x,y,z)(x',y',z')=(x+x',y+y',z+z'+xy').
$$

The subgroup

$$
N=\{(0,y,z):y,z\in\mathbb Z\}
$$

is normal and isomorphic to $\mathbb Z^2$. If $t=(1,0,0)$, then

$$
t(0,y,z)t^{-1}=(0,y,z+y).
$$

Thus, on the coordinate column $(y,z)^T$, [conjugation](../../../../../../conjugation.md) by $t$ is the [linear map](../../../../../../linear-map.md) with matrix

$$
A=\begin{pmatrix}1&0\\1&1\end{pmatrix}.
$$

Every element has a unique expression $(0,y,z)t^x$, so

$$
H\cong\mathbb Z^2\rtimes_A\mathbb Z.
$$

The commutators $[t,(0,y,z)]$ fill the central subgroup of matrices $(0,0,z)$, while the quotient by this subgroup is generated freely and abelianly by the images of $(1,0,0)$ and $(0,1,0)$. Equivalently, $(A-I)\mathbb Z^2$ is the second coordinate axis. Therefore the [abelianization](../../../../../../abelianization.md) is

$$
\boxed{H^{\mathrm{ab}}\cong
\mathbb Z\oplus\mathbb Z^2/(A-I)\mathbb Z^2
\cong\mathbb Z^2.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
