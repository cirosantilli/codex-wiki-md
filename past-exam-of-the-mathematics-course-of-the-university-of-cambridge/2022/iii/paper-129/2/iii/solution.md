<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose $k$ so that

$$
|X|\leq p^k<p|X|
$$

and take a uniformly random codimension-$k$ subspace $V\leq\mathbb F_p^n$. Each fixed nonzero vector lies in $V$ with probability at most $p^{-k}$. The [union bound](../../../../../../boole-s-inequality.md) gives

$$
\mathbb P((X\setminus\{0\})\cap V\ne\varnothing)
\leq(|X|-1)p^{-k}<1.
$$

Thus some $V$ satisfies $V\cap X=\{0\}$.

For a uniformly random coset $W$ of this $V$, every value $\phi(x)$ lies in $W$ with probability $p^{-k}$. Therefore

$$
\mathbb E_W|\phi^{-1}(W)|=p^{-k}p^n,
$$

so some coset has inverse image $A$ of density at least

$$
p^{-k}>\frac1{p|X|}\geq p^{-1}C^{-5}.
$$

Part i says that $\phi|_A$ is a Freiman homomorphism, proving the [large Freiman-homomorphic restriction from bounded derivative images](../../../../../../large-freiman-homomorphic-restriction-from-bounded-derivative-images.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
