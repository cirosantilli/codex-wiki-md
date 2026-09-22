<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\rho:H^*(X;\mathbb Z)\to H^*(X;\mathbb Z/n)$ for coefficient reduction. Compare the two coefficient sequences in part (a): the maps from the integral sequence to the finite sequence are reduction modulo $n$ on the left, reduction modulo $n^2$ in the middle, and the identity on the right. The square involving the injections commutes because $[na]_{n^2}=j([a]_n)$.

Naturality of the [connecting homomorphism](../../../../../../connecting-homomorphism.md) gives the [Bockstein factorization through integral cohomology](../../../../../../bockstein-factorization-through-integral-cohomology.md)

$$
\boxed{\beta=\rho\widehat\beta.}
$$

One can see this directly without a diagram: lift a modulo-$n$ cocycle to an integral cochain $a$. Its coboundary has the form $\delta a=nb$. Then $\widehat\beta[a]=[b]$, whereas $\beta[a]=[b\bmod n]$.

Exactness of the integral coefficient sequence gives $\widehat\beta\rho=0$: a class obtained by reducing an integral cocycle has zero integral connecting class. Consequently

$$
\boxed{\beta^2=\rho\widehat\beta\rho\widehat\beta=0.}
$$

This [Bockstein square-zero identity](../../../../../../bockstein-square-zero-identity.md) holds without requiring $n$ to be prime. At the cochain level, $\delta^2a=0$ and the torsion-free integral cochain groups imply $\delta b=0$, which also makes the second connecting class vanish.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
