<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

For subgroups $H,K\leq G$ and an $H$-representation $W$, [Mackey restriction formula](../../../../../mackey-restriction-formula.md) is

$$
\operatorname{Res}_K^G\operatorname{Ind}_H^G W
\cong
\bigoplus_{x\in K\backslash G/H}
\operatorname{Ind}_{K\cap xHx^{-1}}^K
\operatorname{Res}_{K\cap xHx^{-1}}^{xHx^{-1}}({}^xW).
$$

[Frobenius reciprocity](../../../../../frobenius-reciprocity.md) states

$$
\langle\operatorname{Ind}_H^G\chi,\psi\rangle_G
=\langle\chi,\operatorname{Res}_H^G\psi\rangle_H.
$$

Applying these with $K=H$ gives

$$
\left\langle\operatorname{Ind}_H^G\chi,
\operatorname{Ind}_H^G\chi\right\rangle_G
=
\sum_{x\in H\backslash G/H}
\left\langle
\operatorname{Res}_{H\cap xHx^{-1}}^H\chi,
\operatorname{Res}_{H\cap xHx^{-1}}^{xHx^{-1}}({}^x\chi)
\right\rangle.
$$

The identity double coset contributes one exactly when $W$ is irreducible, and every summand is a nonnegative integer. This proves [Mackey irreducibility criterion](../../../../../mackey-irreducibility-criterion.md): the induced representation is irreducible exactly when $W$ is irreducible and every nonidentity double-coset summand vanishes.

Now take $G=S_n$, $H=S_{n-1}$, and $x=(n-1\ n)\notin H$. Then

$$
H\cap xHx^{-1}=S_{n-2},
$$

the subgroup fixing both $n-1$ and $n$. Conjugation by $x$ fixes every element of this subgroup, so the two representations appearing in the corresponding Mackey summand are both $\operatorname{Res}_{S_{n-2}}^{S_{n-1}}W$. Their inner product is positive because this restriction is nonzero. Hence the [Mackey irreducibility criterion](../../../../../mackey-irreducibility-criterion.md) fails whenever $W$ is irreducible. If $W$ is reducible, induction preserves its direct-sum decomposition, so the induced representation is again reducible. Therefore $\operatorname{Ind}_{S_{n-1}}^{S_n}W$ is never irreducible for $n\geq2$.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
