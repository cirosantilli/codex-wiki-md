<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The commuting [normal operators](../../../../../../normal-operator.md) $T_\ell$, together with the finite-order [diamond operators](../../../../../../diamond-operator.md), admit simultaneous diagonalization for the [Petersson inner product](../../../../../../petersson-inner-product.md). Their restrictions to the [new subspace of cusp forms](../../../../../../new-subspace-of-cusp-forms.md) have one-dimensional common eigenspaces by the [newform multiplicity-one theorem](../../../../../../newform-multiplicity-one-theorem.md). This additional theorem is the essential newform input: normality alone would allow higher multiplicities. Since every $U_p$ commutes with the good-prime operators and preserves the new space, it preserves each such line and is scalar on it. Normalize its nonzero first Fourier coefficient to one to obtain a [newform](../../../../../../newform.md). This gives the requested simultaneous eigenbasis of the new space.

By definition, every old form is a linear combination of lower-level [oldforms by argument dilation](../../../../../../oldform-by-argument-dilation.md). Repeatedly split each lower-level cusp space into its old space and its [Petersson inner product](../../../../../../petersson-inner-product.md) orthogonal new space; induction on the level shows that the specified dilations of [newforms](../../../../../../newform.md) span the full space. To prove independence, separate distinct primitive eigenforms by their good-prime eigenvalues, using the [newform multiplicity-one theorem](../../../../../../newform-multiplicity-one-theorem.md). For a fixed normalized form, its dilations $f(tz)$ are independent: order the distinct positive integers $t$ increasingly, and the coefficient of the least occurring $q^t$ kills its coefficient in any vanishing linear combination. Repeat for the next least $t$. Thus these dilations are indeed a basis.

For trivial character, part (a) shows that $W_N$ commutes with all the good-prime operators, so it preserves the one-dimensional primitive line. Also $W_N^2=(-1)^k$ for the [determinant-normalized slash operator](../../../../../../determinant-normalized-slash-operator.md); a nonzero trivial-character form has even $k$. Therefore

$$
\boxed{W_Nf=\varepsilon f,\qquad\varepsilon\in\{1,-1\}.}
$$

The power of $N$ in an unnormalized Fricke eigenvalue depends on the convention. The plain slash action $(cz+d)^{-k}f(\gamma z)$ gives $\varepsilon N^{-k/2}$, while the Hecke-style action $(\det\gamma)^{k-1}(cz+d)^{-k}f(\gamma z)$ gives $\varepsilon N^{k/2-1}$. The PDF prints $\pm N^{k-1}$; that value requires the deliberate rescaling $w_N=N^{k-1}W_N$ and does not follow under either usual convention. Under that rescaling its displayed eigenvalue is $\varepsilon N^{k-1}$; all the preceding eigenspace and conjugation statements are unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
