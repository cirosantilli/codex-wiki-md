<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a [partial fixed-point logic](../../../../../../partial-fixed-point-logic.md) formula $\phi(R,\mathbf x)$, with $R$ of arity $k$. On a finite ordered structure, an interpretation of $R$ is a bit string of length $n^k$. To decide whether some interpretation makes $\phi$ true at a given tuple, enumerate all these strings and evaluate $\phi$ for each. Evaluation uses [polynomial space](../../../../../../polynomial-space.md) by the permitted characterization of PFP, and the enumerating counter also has polynomial length. Storage is reused between interpretations. Thus the resulting pointed-structure property is decidable in [PSPACE](../../../../../../pspace.md).

Apply the assumed PFP characterization of PSPACE on ordered structures to this property. It gives a PFP formula $\psi(\mathbf x)$ such that

$$
\boxed{\psi(\mathbf x)\equiv\exists R\,\phi(R,\mathbf x)\quad\text{on finite ordered structures}.}
$$

To justify the formula version from a sentence characterization, temporarily name the tuple by finitely many new constants, apply the characterization in that expanded finite signature, and replace those constants by the free variables, renaming bound variables to avoid capture. This does not introduce a new order assumption: the input already interprets $<$ as a [linear order](../../../../../../linear-order.md). Multiple quantified relations are handled by repeated application.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
