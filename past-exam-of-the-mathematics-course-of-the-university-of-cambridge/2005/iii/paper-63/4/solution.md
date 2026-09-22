<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the convention $[e_a,e_c]=C_a{}^b{}_c e_b$, with $C_a{}^b{}_c=-C_c{}^b{}_a$. Expanding the [Jacobi identity](../../../../../jacobi-identity.md) on three basis elements gives

$$
[e_a,[e_b,e_d]]+[e_b,[e_d,e_a]]+[e_d,[e_a,e_b]]=0,
$$

so each coefficient satisfies

$$
C_a{}^e{}_cC_b{}^c{}_d+C_b{}^e{}_cC_d{}^c{}_a+C_d{}^e{}_cC_a{}^c{}_b=0.
$$

Antisymmetry in the input indices makes this equivalent to

$$
\boxed{C_{[a}{}^e{}_{|c|}C_b{}^{|c|}{}_{d]}=0.}
$$

The vertical bars exclude the summed index from antisymmetrization.

In dimension three choose a nonzero contravariant [volume form](../../../../../volume-form.md) $\epsilon^{abc}$ on $\mathfrak g^*$ and its dual $\epsilon_{abc}$, normalized to have component $1$ on an oriented basis. The [three-dimensional Lie algebra structure decomposition](../../../../../three-dimensional-lie-algebra-structure-decomposition.md) starts with

$$
A^{bd}=C_a{}^b{}_c\epsilon^{acd}.
$$

The contraction identifies an antisymmetric pair of indices with one dual index. Every such matrix splits uniquely into its symmetric part $n^{bd}=A^{(bd)}$ and antisymmetric part. The latter has the unique representation

$$
A^{[bd]}=\epsilon^{bde}a_e,\qquad a_e=\frac12\epsilon_{ebd}A^{bd}.
$$

Thus $n$ is a symmetric contravariant tensor and $a$ a covector, and

$$
C_a{}^b{}_c\epsilon^{acd}=n^{bd}+\epsilon^{bde}a_e.
$$

Using $\epsilon_{acd}\epsilon^{ef d}=\delta_a^e\delta_c^f-\delta_a^f\delta_c^e$ gives the inverse formula

$$
C_a{}^b{}_c=\frac12\epsilon_{acd}n^{bd}+\frac12(\delta_c^b a_a-\delta_a^b a_c).
$$

The factors $1/2$ follow from the unnormalized contraction in this particular question.

Only the alternating triple $(e_1,e_2,e_3)$ has to be checked. Substitution of the inverse formula into its Jacobiator gives

$$
[e_1,[e_2,e_3]]+[e_2,[e_3,e_1]]+[e_3,[e_1,e_2]]=-\frac12n^{be}a_e e_b.
$$

One can see the cancellation explicitly by using an auxiliary positive inner product and diagonalizing the symmetric matrix $n$ by an orientation-preserving orthogonal change of basis. If its diagonal entries are $n_1,n_2,n_3$, the brackets are

$$
[e_2,e_3]=\tfrac12(n_1e_1+a_2e_3-a_3e_2),\quad
[e_3,e_1]=\tfrac12(n_2e_2+a_3e_1-a_1e_3),\quad
[e_1,e_2]=\tfrac12(n_3e_3+a_1e_2-a_2e_1).
$$

In their Jacobiator, the terms involving two $n$'s or two $a$'s cancel and the remaining terms are $-\tfrac12(n_1a_1e_1+n_2a_2e_2+n_3a_3e_3)$. Returning to the original basis proves the displayed formula. Therefore

$$
\boxed{\text{Jacobi holds if and only if }n^{ae}a_e=0.}
$$

This imposes three algebraic conditions on the nine independent entries of the original antisymmetric structure constants; if $a\ne0$, it must lie in the kernel of $n$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
