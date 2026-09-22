<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Replace the open [knot complement](../../../../../knot-exterior.md) by the compact [knot exterior](../../../../../knot-exterior.md) $E_K$; they have the same [homotopy type](../../../../../homotopy-type.md). The [abelianization](../../../../../abelianization.md)

$$
\pi_1(E_K)\longrightarrow H_1(E_K;\mathbb Z)\cong\mathbb Z
$$

sends an oriented [meridian of a knot](../../../../../meridian-of-a-knot.md) to $1$. The connected [covering space](../../../../../covering-space.md) corresponding to its kernel is the [infinite cyclic cover of a knot exterior](../../../../../infinite-cyclic-cover-of-a-knot-exterior.md) $\widetilde E_K$. Choose a generator $t$ of its [deck transformation group](../../../../../deck-transformation-group.md). Then

$$
\mathcal A_K=H_1(\widetilde E_K;\mathbb Z)
$$

is the [Alexander module of a knot](../../../../../alexander-module-of-a-knot.md) over $\Lambda=\mathbb Z[t,t^{-1}]$. It is a finitely presented torsion [module](../../../../../module-mathematics.md), and its order, equivalently the greatest common divisor of the appropriate maximal [matrix minors](../../../../../minor-linear-algebra.md) of an [Alexander matrix](../../../../../alexander-matrix.md), is the [Alexander polynomial of a knot](../../../../../alexander-polynomial.md), up to a [unit](../../../../../unit-in-a-ring.md) $\pm t^m$.

For a [fibered knot](../../../../../fibered-knot.md), the [infinite cyclic cover of a knot exterior](../../../../../infinite-cyclic-cover-of-a-knot-exterior.md) is $\Sigma\times\mathbb R$. Write the [mapping torus](../../../../../mapping-torus.md) with the gluing convention in the question. The [deck transformation](../../../../../deck-transformation.md)

$$
D(x,s)=(\phi(x),s-1)
$$

has exactly that quotient: $(x,1)$ and $(\phi(x),0)$ are identified. Choose $t=D$. Its action on $H_1(\Sigma;\mathbb Z)$ is $\phi_*$. If one instead chooses the generator projecting in the positive circle direction, its action is $\phi_*^{-1}$; this replaces $t$ by $t^{-1}$ and produces an associate for a knot.

Choose an integral basis for $H_1(\Sigma)\cong\mathbb Z^{2g}$ and let $\Phi$ be the [matrix](../../../../../matrix.md) of $\phi_*$. The [Alexander module of a knot](../../../../../alexander-module-of-a-knot.md) has the finite free module presentation

$$
\Lambda^{2g}\xrightarrow{\,tI-\Phi\,}\Lambda^{2g}\longrightarrow\mathcal A_K\longrightarrow0.
$$

There are no further relations: using $t v=\Phi v$ and the invertibility of $\Phi$, every Laurent combination reduces uniquely to an integral combination of the chosen basis elements. Taking the order of this square presentation gives the **monodromy formula**

$$
\boxed{\Delta_K(t)\doteq\det(tI-\phi_*).}
$$

For a disk fiber both sides are $1$, using the empty [determinant](../../../../../determinant.md) convention.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
