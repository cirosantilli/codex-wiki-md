<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $n=|\Omega|\geq2$, and let $H=G_\alpha$. Sharp two-transitivity gives $|G|=n(n-1)$ and $|H|=n-1$. A nonidentity element fixes at most one point. Counting the nonidentity elements in the $n$ [stabilizer subgroups](../../../../../../stabilizer-subgroup.md) shows that there are $n-1$ fixed-point-free elements. Let $N$ be this set together with the identity. We first prove it is a [normal subgroup](../../../../../../normal-subgroup.md), rather than presuming that fixed-point-free elements are closed under multiplication.

For $n=2$, $G=C_2$ and $N=G$ directly. Otherwise use complex [characters of a finite group](../../../../../../character-of-a-representation.md). Let $\pi$ be the [permutation character](../../../../../../permutation-character.md) and $\psi=\pi-1$, the character of the [permutation representation](../../../../../../permutation-representation.md) with its constant line removed. For every nontrivial [irreducible character](../../../../../../irreducible-character.md) $\theta$ of $H$, form the [virtual character](../../../../../../virtual-character.md)

$$
\varphi_\theta=\operatorname{Ind}_H^G\theta-\theta(1)\psi.
$$

Its values are $\theta(1)$ at the identity and at every fixed-point-free element. At an element with one fixed point, conjugate it to $h\in H\setminus\{1\}$; induction gives $\varphi_\theta(g)=\theta(h)$, because there is exactly one fixed coset.

The identity and the $n-1$ fixed-point-free elements together contribute $n\theta(1)\overline{\eta(1)}$ to the inner product. The remaining elements are partitioned into the nonidentity parts of the $n$ [stabilizer subgroups](../../../../../../stabilizer-subgroup.md). Hence [character orthogonality](../../../../../../character-orthogonality.md) gives

$$
\langle\varphi_\theta,\varphi_\eta\rangle_G
=\frac{n}{|G|}\sum_{h\in H}\theta(h)\overline{\eta(h)}
=\delta_{\theta,\eta}.
$$

A [virtual character](../../../../../../virtual-character.md) of norm one is plus or minus an [irreducible character](../../../../../../irreducible-character.md): its coefficients in the irreducible-character basis are integers whose squares sum to one. Its positive degree $\theta(1)$ selects the plus sign. Thus each $\varphi_\theta$ is an actual [irreducible character](../../../../../../irreducible-character.md).

For a [group representation](../../../../../../group-representation.md), $\chi(g)=\chi(1)$ holds exactly on its kernel: make the representation unitary and compare the sum of its unit-modulus eigenvalues with its dimension. All of $N$ therefore lies in the intersection of the kernels of the $\varphi_\theta$. Conversely, a nonidentity element fixing a point gives $h\ne1$ in $H$. Some nontrivial [irreducible character](../../../../../../irreducible-character.md) of $H$ has $\theta(h)\ne\theta(1)$, since otherwise the [regular representation](../../../../../../regular-representation.md) of $H$ would not vanish at $h$. Consequently

$$
N=\bigcap_{\theta\ne1_H}\ker\varphi_\theta.
$$

This proves normality and subgroup closure. It has order $n$ and no nonidentity element fixing a point, so it is a [regular permutation subgroup](../../../../../../regular-permutation-subgroup.md).

Now $H$ acts transitively by conjugation on $N\setminus\{1\}$: identify an element of $N$ with its image of $\alpha$ and use transitivity of $H$ on the remaining points. Thus all nonidentity elements of $N$ have the same order. Taking a suitable power of one element shows this common order is a prime $p$. By Cauchy's theorem no other prime divides $|N|$, so $N$ is a $p$-group. Its nontrivial center is $H$-invariant, so transitivity forces the center to be all of $N$. Therefore $N$ is [elementary abelian](../../../../../../elementary-abelian-group.md) of order $p^d=n$.

Since $|H|=p^d-1$ is prime to $p$, $N$ is the unique Sylow $p$-subgroup of $G$. Uniqueness makes it characteristic under every [group automorphism](../../../../../../group-automorphism.md). We have proved

$$
\boxed{N\text{ is regular, elementary abelian and characteristic in }G.}
$$

The character argument supplies the [regular kernel of a finite sharply two-transitive group](../../../../../../regular-kernel-of-a-finite-sharply-two-transitive-group.md); the final Sylow argument establishes the stronger characteristic assertion.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
