<h1 id="19j/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $a\in\mathbb F_p^*$ put

$$
t(a)=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}.
$$

Conjugation gives

$$
t(a)u(x)t(a)^{-1}=u(a^2x).
$$

Suppose the $\chi$-weight space

$$
V_\chi=\{z\in V:u(x)z=\chi(u(x))z\text{ for all }x\}
$$

is nonzero. If $0\ne z\in V_\chi$, then $t(a)z$ lies in the $\chi(a^{-2}\mathbin\cdot)$-weight space, because

$$
u(x)t(a)z
=t(a)u(a^{-2}x)z
=\chi(u(a^{-2}x))t(a)z.
$$

Hence every character indexed by a nonzero square occurs in $\operatorname{Res}_U^BV$.

These characters are distinct. Indeed, if $\chi(v\mathbin\cdot)=\chi(v'\mathbin\cdot)$ with $v\ne v'$, multiplication by $v-v'$ would show that $\chi$ is trivial on all of $U$, contrary to hypothesis. There are $(p-1)/2$ nonzero squares, so

$$
\left\langle\operatorname{Res}_U^BV,\chi(v\mathbin\cdot)\right\rangle_U\ne0
$$

for at least $(p-1)/2$ values of $v\in\mathbb F_p^*$. This is the [square orbits of additive characters of a finite field](../../../../../../../square-orbits-of-additive-characters-of-a-finite-field.md) argument.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [19J](../../../19j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
