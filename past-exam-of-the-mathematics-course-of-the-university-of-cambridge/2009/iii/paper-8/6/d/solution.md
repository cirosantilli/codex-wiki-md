<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Amplify the chiral phase by the identity on the auxiliary $\mathbb C^2$, and let $P$ act by multiplication on each chirality. The displayed projection has image line $E_z=\mathbb C(1,\overline z)$. On the chart $w=1/z$ near infinity it has frame $(\overline w,1)$. On the equator the normalized second frame is $z$ times the first, so its clutching function has winding $+1$. Equivalently it is the conjugate of the tautological degree-$-1$ line. Thus $E$ has degree $+1$ with the complex orientation fixed in part (c).

It is equivariant for the conjugate defining action on the auxiliary $\mathbb C^2$; this representation is equivalent to the defining representation of $SU(2)$. At $z=0$ its isotropy character under $\operatorname{diag}(e^{it},e^{-it})$ is $e^{-it}$. Tensoring with the positive spinor weight $+1$ gives weight zero on $S^+\otimes E$, whereas tensoring with the negative weight $-1$ gives weight $-2$ on $S^-\otimes E$.

The compressed map is

$$
PVP:P(H_+\otimes\mathbb C^2)\longrightarrow P(H_-\otimes\mathbb C^2).
$$

Its parametrix is $PV^*P$: the two products equal the respective identity $P$ modulo compacts, since every matrix entry of $P$ is a continuous function and the phase commutators in part (c) are compact. Hence this is an equivariant [Fredholm operator](../../../../../../fredholm-operator.md).

Use the precisely stated homogeneous-bundle multiplicity rule from part (c). The domain, of weight zero, decomposes as $E_0\oplus E_2\oplus E_4\oplus\cdots$. The target, of weight $-2$, decomposes as $E_2\oplus E_4\oplus\cdots$. Part (b) subtracts these multiplicities, leaving only the trivial representation. Therefore

$$
\boxed{\operatorname{ind}_G(PVP)=[E_0],\qquad\operatorname{ind}(PVP)=1.}
$$

This computes the index from the actual projection and representation weights without invoking an index theorem that merely supplies the requested number. Reversing the chiral direction gives $-1$. If $V$ instead denotes the full self-adjoint phase on $H_+\oplus H_-$, its compression is self-adjoint [Fredholm](../../../../../../fredholm-operator.md) and has index zero; the nonzero answer uses the standard chiral interpretation made explicit above.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
