<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

As usual, a class of structures here is closed under isomorphism and uses standard finite-structure encodings. First suppose $K$ is defined by $\exists R\,\phi$, with $\phi$ in [partial fixed-point logic](../../../../../../partial-fixed-point-logic.md). Deterministically enumerate the polynomial-length encodings of $R$ and evaluate $\phi$ on each expansion. PFP evaluation is in [PSPACE](../../../../../../pspace.md) even without a supplied order: a relation of fixed arity requires polynomially many bits, iteration has at most exponentially many states, and a polynomial-length counter suffices to stop after that many stages. If no consecutive stages agree before a repeat must have occurred, the partial fixed point is empty. Nested fixed points have fixed syntactic depth and can be evaluated with reused polynomial storage. Thus the encoding language of $K$ is in PSPACE.

Conversely, suppose that encoding language is decidable in PSPACE. Expand each structure by a freely chosen [linear order](../../../../../../linear-order.md) $R$. On such ordered expansions, the assumed characterization gives a PFP sentence $\psi(R)$ deciding whether the reduct belongs to $K$. Since $K$ is isomorphism-invariant, the answer is independent of the particular chosen order. Hence

$$
\boxed{A\in K\quad\Longleftrightarrow\quad
A\models\exists R\,[\operatorname{Lin}(R)\land\psi(R)].}
$$

The expression inside the second-order quantifier is PFP, since the assertion that $R$ is a [linear order](../../../../../../linear-order.md) is first-order. Every finite universe has a [linear order](../../../../../../linear-order.md). This proves both directions, using an existentially supplied order when the original signature has none. The construction is also the order-independent consequence of part (a), which shows that existential relation quantification does not increase PFP's power on an already ordered structure.

## ↑ Ancestors (11)

1. [B](../b.md)
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
