<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [highest-weight vector](../../../../../../highest-weight-vector.md) is a nonzero [weight vector](../../../../../../weight-vector.md) $v$ such that $\mathfrak g_\alpha v=0$ for every [positive root](../../../../../../positive-root.md) $\alpha$. Its [weight of a representation](../../../../../../weight-of-a-representation.md) is a highest weight. For an irreducible finite-dimensional [Lie algebra representation](../../../../../../lie-algebra-representation.md), this is the unique [highest weight of a representation](../../../../../../highest-weight-of-a-representation.md), and $v$ generates the module; a reducible module can have several highest weights of different summands.

Here is an existence argument for every nonzero finite-dimensional module $V$. For each [simple root](../../../../../../simple-root.md), its root operators and [coroot](../../../../../../coroot.md) form an [sl2 subalgebra associated with a root](../../../../../../sl2-subalgebra-associated-with-a-root.md). The [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md) shows that this coroot acts diagonalizably with integral [eigenvalues](../../../../../../eigenvalue.md). These commuting coroots span the [Cartan subalgebra](../../../../../../cartan-subalgebra.md), so simultaneous diagonalization gives a finite [weight-space decomposition](../../../../../../weight-space-decomposition.md)

$$
V=\bigoplus_\lambda V_\lambda.
$$

Choose a real linear functional $\ell$ on the [weight lattice](../../../../../../weight-lattice.md) span that is positive on every [simple root](../../../../../../simple-root.md), hence on every [positive root](../../../../../../positive-root.md), and choose a weight $\lambda$ maximizing $\ell$ among the finitely many weights of $V$. If $v\in V_\lambda$ and $X_\alpha\in\mathfrak g_\alpha$, then

$$
H(X_\alpha v)=X_\alpha Hv+[H,X_\alpha]v=(\lambda(H)+\alpha(H))X_\alpha v,
$$

so $X_\alpha v$ belongs to $V_{\lambda+\alpha}$ if nonzero. For positive $\alpha$, that would contradict maximality because $\ell(\lambda+\alpha)>\ell(\lambda)$. Thus every nonzero $v\in V_\lambda$ is a [highest-weight vector](../../../../../../highest-weight-vector.md). **Every nonzero finite-dimensional module therefore has a highest weight.** The zero module has no nonzero vector or weight, so it is the vacuous exception to the literal unrestricted wording.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
