<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose positive roots

$$
\Phi^+=\{\varepsilon_1-\varepsilon_2,\varepsilon_2,
\varepsilon_1,\varepsilon_1+\varepsilon_2\}.
$$

The corresponding simple roots are $\varepsilon_1-\varepsilon_2$ and $\varepsilon_2$. The vector $v_{1,+}\wedge v_{2,+}$ has weight $\lambda=\varepsilon_1+\varepsilon_2$. Adding any positive root to this weight produces a weight absent from part (a), so every positive root vector annihilates it. It is consequently a [highest-weight vector](../../../../../../highest-weight-vector.md) with highest weight $\lambda$.

A representation of a [compact Lie group](../../../../../../compact-lie-group.md) is completely reducible: Haar averaging makes an inner product invariant, and orthogonal complements of invariant subspaces remain invariant. Therefore the [exterior square](../../../../../../exterior-square.md) contains an irreducible summand $L_\lambda$ of this highest weight. This can also be seen by projecting the displayed highest-weight vector into irreducible summands; a nonzero projection remains annihilated by all positive root vectors and has the same weight. Its multiplicity is one because the weight space at $\lambda$ is one-dimensional.

Use the [Weyl dimension formula](../../../../../../weyl-dimension-formula.md), expressly allowed in this part:

$$
\dim L_\lambda=\prod_{\alpha\in\Phi^+}
\frac{\langle\lambda+\rho,\alpha\rangle}{\langle\rho,\alpha\rangle}.
$$

Here $L_\lambda$ is the irreducible highest-weight representation, $\Phi^+$ is the chosen positive root system, $\rho$ is half its sum, and the pairing is the invariant Euclidean inner product on the real weight plane, with $\varepsilon_1,\varepsilon_2$ orthonormal. Using coroots instead gives the same ratio because the length factor cancels for each root. In this convention,

$$
\rho=\tfrac32\varepsilon_1+\tfrac12\varepsilon_2,
\qquad\lambda+\rho=\tfrac52\varepsilon_1+\tfrac32\varepsilon_2.
$$

The four factors, in the listed positive-root order, are respectively

$$
\frac{1}{1},\qquad\frac{3/2}{1/2},\qquad
\frac{5/2}{3/2},\qquad\frac{4}{2}.
$$

Their product is $10$. Since $\dim\Lambda^2\mathbb C^5=\binom52=10$, this irreducible summand occupies the entire exterior square. Hence

$$
\boxed{\Lambda^2\mathbb C^5\text{ is irreducible as an }SO(5)\text{-representation}.}
$$

The proof uses the dimension formula only where it is allowed, not in the symmetric-power argument of Question 2. Its [B2 adjoint representation weight diagram](../../../../../../b2-adjoint-representation-weight-diagram.md) is exactly the eight roots and the double zero weight obtained above.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
