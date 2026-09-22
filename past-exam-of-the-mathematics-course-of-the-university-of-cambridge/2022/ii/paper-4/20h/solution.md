<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Two nonzero [fractional ideals](../../../../../fractional-ideal.md) $I,J$ of $\mathcal O_K$ are in the same ideal class when

$$
I=(\alpha)J
$$

for some $\alpha\in K^\times$, equivalently when $IJ^{-1}$ is principal. Multiplication is well defined on classes:

$$
[I][J]=[IJ].
$$

The identity is $[\mathcal O_K]$, the inverse of $[I]$ is $[I^{-1}]$, and commutativity comes from ideal multiplication. Nonzero fractional ideals are invertible because $\mathcal O_K$ is a Dedekind domain. Thus these classes form the abelian [ideal class group](../../../../../ideal-class-group.md) $\operatorname{Cl}(K)$.

For finiteness, begin with a nonzero integral ideal $I$. By hypothesis choose $0\ne\alpha\in I$ with

$$
|N_{K/\mathbb Q}(\alpha)|\leq c_KN(I).
$$

Since $(\alpha)\subseteq I$, the ideal

$$
J=(\alpha)I^{-1}
$$

is integral, represents $[I]^{-1}$, and satisfies

$$
N(J)
=\frac{|N_{K/\mathbb Q}(\alpha)|}{N(I)}
\leq c_K.
$$

Hence every class has an integral representative of bounded norm. There are only finitely many integral ideals of bounded norm, so $\operatorname{Cl}(K)$ is finite. This is the [bounded-norm ideal representatives](../../../../../bounded-norm-ideal-representatives.md) argument.

Now take $K=\mathbb Q(\sqrt{-33})$. Since $-33\equiv3\pmod4$,

$$
\mathcal O_K=\mathbb Z[\sqrt{-33}],
\qquad
d_K=-132.
$$

The imaginary-quadratic [Minkowski bound for ideal classes](../../../../../minkowski-s-bound.md) is

$$
\frac2\pi\sqrt{|d_K|}
=\frac2\pi\sqrt{132}<8.
$$

Every class is therefore represented by an integral ideal of norm at most seven.

The ramified prime ideals above two and three are

$$
\mathfrak p_2=(2,1+\sqrt{-33}),
\qquad
\mathfrak p_3=(3,\sqrt{-33}),
$$

with

$$
\mathfrak p_2^2=(2),
\qquad
\mathfrak p_3^2=(3).
$$

Neither is principal, since the norm equation

$$
a^2+33b^2=2\quad\text{or}\quad3
$$

has no integer solution. Their product is also nonprincipal, since $a^2+33b^2=6$ has no solution. Thus

$$
1,\quad[\mathfrak p_2],\quad[\mathfrak p_3],
\quad[\mathfrak p_2\mathfrak p_3]
$$

are four distinct classes, all of order at most two.

The prime five is inert, so it contributes no ideal of norm five. The prime seven splits as

$$
\mathfrak q_\pm=(7,\sqrt{-33}\mp3).
$$

Since

$$
(3+\sqrt{-33})
=\mathfrak p_2\mathfrak p_3\mathfrak q_-,
$$

comparison of norms, all equal to $42$, confirms the factorization and gives

$$
[\mathfrak q_-]=[\mathfrak p_2\mathfrak p_3].
$$

The conjugate prime has the inverse class, which is the same because this class has order two. Ideals of norms four and six yield respectively the principal class and $[\mathfrak p_2\mathfrak p_3]$. The Minkowski bound now shows that the four displayed classes exhaust the group. Therefore

$$
\boxed{
\operatorname{Cl}(\mathbb Q(\sqrt{-33}))
\cong C_2\times C_2
}.
$$

This is the [Ideal class group of Q of square root of minus thirty-three](../../../../../ideal-class-group-of-q-of-square-root-of-minus-thirty-three.md).

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
