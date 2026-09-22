<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Realize $\xi^\lambda$ as the permutation character on ordered set partitions with row sizes $\lambda_1,\lambda_2,\ldots$. Under $S_m\times S_k$, an orbit is determined by the weak composition $\mu$ whose $i$th part counts elements of $\{m+1,\ldots,n\}$ in row $i$. Its stabilizer is the product of the Young subgroups for $\lambda-\mu$ and $\mu$. The orbit character is therefore the outer tensor product $\xi^{\lambda-\mu}\mathbin\#\xi^\mu$, and summing the orbits gives

$$
\left.\xi^\lambda\right\downarrow_{S_m\times S_k}
=\sum_{\mu\models k}\xi^{\lambda-\mu}\mathbin\#\xi^\mu,
$$

with impossible compositions contributing zero.

Insert this identity into the alternating definition of $\psi^\lambda$. Group the weak compositions by permutations of their parts and use [character straightening](../../../../../../straightening-of-a-symmetric-group-character-indexed-by-a-composition.md); the alternating sum in the first tensor factor is $\psi^{\lambda-\mu}$, while the second factors combine once for each partition $\mu\vdash k$. Thus

$$
\boxed{\left.\psi^\lambda\right\downarrow_{S_m\times S_k}
=\sum_{\mu\vdash k}\psi^{\lambda-\mu}\mathbin\#\xi^\mu.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 160](../../../paper-160-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
