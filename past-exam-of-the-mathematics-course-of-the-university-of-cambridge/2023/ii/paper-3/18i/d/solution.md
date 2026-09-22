<h1 id="18i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a primitive root $\zeta_n$. Since every root of $\Phi_n$ is a power of $\zeta_n$, its splitting field is $L=K(\zeta_n)$. Each $\sigma\in G$ sends $\zeta_n$ to another primitive root, uniquely of the form

$$
\sigma(\zeta_n)=\zeta_n^{a_\sigma},
\qquad
a_\sigma\in(\mathbb Z/n\mathbb Z)^\times.
$$

The assignment $\sigma\mapsto a_\sigma$ is a homomorphism. It is injective because an automorphism fixing $\zeta_n$ fixes $K(\zeta_n)=L$.

If $\Phi_n$ is irreducible over $K$, the orbit of $\zeta_n$ has all $\varphi(n)$ primitive roots, so the injection has image of size $\varphi(n)$ and is surjective. Conversely, surjectivity makes every primitive root a conjugate of $\zeta_n$. Its minimal polynomial over $K$ then has at least $\varphi(n)$ roots and divides the degree-$\varphi(n)$ polynomial $\Phi_n$, so it equals $\Phi_n$. This proves the [Galois embedding for a cyclotomic polynomial](../../../../../../galois-embedding-for-a-cyclotomic-polynomial.md) and the claimed equivalence.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [18I](../../18i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
