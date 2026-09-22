<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Measure the [coset state](../../../../../../../coset-state.md) in the common [eigenbasis](../../../../../../../eigenbasis.md) $\{|v_\chi\rangle\}$ of the [group shift operators](../../../../../../../group-shift-operator.md). Its overlap is

$$
\langle v_\chi|g_0+K\rangle
=\frac{\chi(g_0)}{\sqrt{|G||K|}}\sum_{k\in K}\chi(k).
$$

The [character-sum cancellation lemma](../../../../../../../character-sum-cancellation-lemma.md) makes this sum $|K|$ when $\chi$ is trivial on $K$, and zero otherwise. Hence, with $K^\perp$ the [annihilator of a subgroup of a finite abelian group](../../../../../../../annihilator-of-a-subgroup-of-a-finite-abelian-group.md),

$$
\boxed{\Pr(\chi)=\begin{cases}|K|/|G|,&\chi\in K^\perp,\\0,&\chi\notin K^\perp.\end{cases}}
$$

Since $|K^\perp|=|G|/|K|$, this is the [uniform distribution on a finite set](../../../../../../../discrete-uniform-distribution.md) $K^\perp$. The factor $\chi(g_0)$ has [modulus](../../../../../../../modulus.md) one, so the distribution is independent of $g_0$. This is [abelian hidden-subgroup Fourier sampling](../../../../../../../abelian-hidden-subgroup-fourier-sampling.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
