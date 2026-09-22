<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $e,h,f$ for the standard generators of the [sl2 Lie algebra](../../../../../../../sl2-lie-algebra.md). For the representation $\phi$, use the normalization

$$
\Omega=\phi(e)\phi(f)+\phi(f)\phi(e)+\frac12\phi(h)^2.
$$

This is the quadratic [Casimir element](../../../../../../../casimir-element.md), and by assumption it commutes with every $\phi(x)$.

[Schur lemma](../../../../../../../schur-s-lemma.md) says that an endomorphism of a finite-dimensional irreducible complex representation which commutes with the representation is a scalar. Hence $\Omega=cI_V$ when $V$ is irreducible.

Let $v$ be a [highest-weight vector](../../../../../../../highest-weight-representation.md) of highest weight $m$, so $ev=0$ and $hv=mv$. Since $[e,f]=h$,

$$
efv=(fe+h)v=mv,
\qquad fev=0.
$$

Therefore

$$
\Omega v=\left(m+\frac12m^2\right)v
=\frac12m(m+2)v.
$$

It follows from scalarity that

$$
\boxed{\Omega=\frac12m(m+2)I_V}.
$$

This is the [Casimir eigenvalue for sl2](../../../../../../../casimir-eigenvalue-for-sl2.md) in the chosen normalization.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 102](../../../../paper-102-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
