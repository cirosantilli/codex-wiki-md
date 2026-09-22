<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Split the sequence as vector spaces at each vertex. In these coordinates, the middle arrow maps have block form

$$
f^Y_\rho=\begin{pmatrix}f^X_\rho&\xi_\rho\\0&f^Z_\rho\end{pmatrix}.
$$

For $t\in k^\times$, change basis by $\operatorname{diag}(tI_{X_i},I_{Z_i})$ at every vertex. It changes the off-diagonal block to $t\xi_\rho$. These arrow matrices depend polynomially on $t$ and at $t=0$ give $X\oplus Z$. Thus the [split extension as a degeneration](../../../../../../split-extension-as-a-degeneration.md) shows

$$
\mathcal O_{X\oplus Z}\subseteq\overline{\mathcal O_Y}.
$$

We must check that the two orbits are different. If $Y\cong X\oplus Z$, apply $\operatorname{Hom}_Q(Z,-)$ to the original [short exact sequence](../../../../../../short-exact-sequence.md). Exactness makes the kernel of $\operatorname{Hom}(Z,Y)\to\operatorname{End}(Z)$ equal to $\operatorname{Hom}(Z,X)$. The assumed isomorphism of the middle representation gives $\dim\operatorname{Hom}(Z,Y)=\dim\operatorname{Hom}(Z,X)+\dim\operatorname{End}(Z)$, so this map is surjective. In particular the identity of $Z$ lifts to $Z\to Y$, splitting the sequence, a contradiction. Hence the orbits are indeed distinct.

The group $\operatorname{GL}(\mathbf n)$ is irreducible, so $\overline{\mathcal O_Y}$ is irreducible. An algebraic-group orbit is locally closed, hence open in its closure; its boundary is a proper closed subset of smaller dimension. The distinct orbit $\mathcal O_{X\oplus Z}$ lies in that boundary. Therefore

$$
\boxed{\dim\mathcal O_{X\oplus Z}<\dim\mathcal O_Y.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
