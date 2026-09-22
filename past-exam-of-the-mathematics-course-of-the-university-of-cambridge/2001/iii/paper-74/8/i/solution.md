<h1 id="8/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The hypotheses make $K$ a [CM-field](../../../../../../cm-field.md), with nontrivial automorphism $c$ over the [totally real number field](../../../../../../totally-real-number-field.md) $k$. In every complex embedding of $K$, this automorphism acts as [complex conjugation](../../../../../../complex-conjugation.md). Write $E_K=\mathcal O_K^\times$, $E_k=\mathcal O_k^\times$ and $\mu_K$ for the finite cyclic group of [roots of unity](../../../../../../root-of-unity.md) in $K$.

For any $u\in E_K$, the element $u/c(u)$ is an algebraic integer, indeed a unit, and every conjugate has absolute value one. The [Kronecker theorem on algebraic integers in the unit disk](../../../../../../kronecker-theorem-on-algebraic-integers-in-the-unit-disk.md) makes it a root of unity. For clarity, the essential proof is finite: the conjugates of all positive powers have modulus one, so the integer coefficients of their monic minimal polynomials are bounded by fixed binomial coefficients. There are only finitely many such polynomials and roots; two powers coincide, forcing a root of unity.

Thus

$$
\phi:E_K\longrightarrow\mu_K,\qquad\phi(u)=u/c(u)
$$

is a homomorphism. Its kernel is exactly $E_k$, since a conjugation-fixed element lies in $k$ and both it and its inverse are integral there. For $\zeta\in\mu_K$, $c(\zeta)=\zeta^{-1}$ and $\phi(\zeta)=\zeta^2$. Consequently $\phi$ induces an injection

$$
E_K/(E_k\mu_K)\hookrightarrow\mu_K/\mu_K^2.
$$

To check injectivity explicitly, if $\phi(u)=\zeta^2$, then $\phi(u/\zeta)=1$, so $u/\zeta\in E_k$. The cyclic group $\mu_K$ has even order because it contains $-1$, and its quotient by squares has order two. Therefore the [unit index of a CM-field](../../../../../../unit-index-of-a-cm-field.md) satisfies

$$
\boxed{[E_K:E_k\mu_K]\in\{1,2\}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8](../../8.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
