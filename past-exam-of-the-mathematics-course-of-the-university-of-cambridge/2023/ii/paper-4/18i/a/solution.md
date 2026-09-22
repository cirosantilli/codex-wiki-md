<h1 id="18i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If a monic [polynomial](../../../../../../polynomial-split.md) $f$ has roots $\alpha_1,\ldots,\alpha_n$ in a [splitting field](../../../../../../splitting-field.md), its [polynomial discriminant](../../../../../../polynomial-discriminant.md) is

$$
\operatorname{disc}(f)
=\prod_{1\leq i<j\leq n}(\alpha_i-\alpha_j)^2.
$$

It is a symmetric polynomial in the roots, so it belongs to the base [field](../../../../../../field.md); it is nonzero exactly when $f$ is a [separable polynomial](../../../../../../separable-polynomial.md).

Put

$$
D=\prod_{i<j}(\alpha_i-\alpha_j),
$$

the [Vandermonde determinant](../../../../../../vandermonde-determinant.md). A root permutation $\sigma$ sends $D$ to $\operatorname{sgn}(\sigma)D$. Hence the [Galois group of a polynomial](../../../../../../galois-group-of-a-polynomial.md) is contained in the [alternating group](../../../../../../alternating-group.md) $A_n$ exactly when every Galois automorphism fixes $D$, which by the fixed-field property is equivalent to $D\in K$. This implies that $\operatorname{disc}(f)=D^2$ is a square in $K$. Conversely, if $\operatorname{disc}(f)=d^2$ for $d\in K$, then $D^2=d^2$, so $D=\pm d\in K$. The Galois group therefore fixes $D$ and consists of even permutations. This proves the [discriminant criterion for an alternating Galois group](../../../../../../discriminant-criterion-for-an-alternating-galois-group.md).

Now let

$$
f(T)=T^3-2T+2.
$$

The [rational root theorem](../../../../../../rational-root-theorem.md) shows that none of $\pm1,\pm2$ is a root, so this cubic is irreducible over $\mathbb Q$. The [discriminant of a depressed cubic](../../../../../../discriminant-of-a-depressed-cubic.md) is

$$
\operatorname{disc}(f)
=-4(-2)^3-27(2)^2
=32-108=-76=-4\cdot19.
$$

This is not a square in $\mathbb Q$, so the [Galois group of an irreducible cubic](../../../../../../galois-group-of-an-irreducible-cubic.md) is $S_3$ over $\mathbb Q$.

Over $K=\mathbb Q(\sqrt{-19})$, the discriminant is the square

$$
-76=(2\sqrt{-19})^2.
$$

The cubic remains irreducible: a root in the degree-two extension $K/\mathbb Q$ would generate over $\mathbb Q$ both a degree-three field, by irreducibility, and a subfield of a degree-two field, contradicting the [tower law for field extensions](../../../../../../tower-law-for-field-extensions.md). Its Galois group over $K$ is consequently $A_3\cong C_3$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18I](../../18i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
