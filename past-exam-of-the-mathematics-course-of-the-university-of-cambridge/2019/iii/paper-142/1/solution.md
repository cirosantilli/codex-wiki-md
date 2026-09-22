<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a compact space $X$, $K^0(X)$ is the [Grothendieck group](../../../../../grothendieck-group.md) of isomorphism classes of finite-rank complex [vector bundles](../../../../../vector-bundle.md) under direct sum. Tensor product descends to this group and makes it a ring, with $[\mathbb C_X]$ as its unit.

The hypothesis $E_0\oplus\mathbb C_X\cong E_1\oplus\mathbb C_X$ says that $E_0$ and $E_1$ define the same stable class. Rank-$d$ bundles are classified by maps to $BU(d)$, and the stabilization $BU(d)\to BU$ is $2d$-connected. Since the finite [CW complex](../../../../../cw-complex.md) $X$ has dimension $k\leq2d$, stabilization is injective on $[X,BU(d)]$. Thus [stable cancellation for complex vector bundles](../../../../../stable-cancellation-for-complex-vector-bundles.md) gives

$$
\boxed{E_0\cong E_1.}
$$

Now let $E_0,E_1$ have rank $d$ over [Complex projective space](../../../../../complex-projective-space.md) $\mathbb{CP}^d$ and have the same [Chern classes](../../../../../chern-class.md). Their [Chern characters](../../../../../chern-character.md) agree because each component of $\operatorname{ch}(E)$ is a universal rational polynomial in the Chern classes. The ring

$$
K^0(\mathbb{CP}^d)\cong\mathbb Z[t]/(t^{d+1})
$$

is torsion-free, while the Chern character becomes an isomorphism after tensoring with $\mathbb Q$; it is therefore injective. Hence $[E_0]=[E_1]$ in K-theory, so after adding trivial bundles they are isomorphic. Since $\mathbb{CP}^d$ has real dimension $2d$, cancellation applies once more:

$$
\boxed{c(E_0)=c(E_1)\Longrightarrow E_0\cong E_1.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
