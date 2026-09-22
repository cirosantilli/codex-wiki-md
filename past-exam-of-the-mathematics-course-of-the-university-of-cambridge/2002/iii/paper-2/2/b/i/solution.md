<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose first that $N$ is the [Frobenius kernel](../../../../../../../frobenius-kernel.md). An element $g\notin N$ fixes a point in the Frobenius action. If $n\in C_N(g)$, then $n$ maps that point to another point fixed by $g$. Since $g$ has only one fixed point and $N$ acts regularly, $n=1$. Thus

$$
C_N(g)=1\qquad(g\notin N).
$$

No nonidentity [conjugacy class](../../../../../../../conjugacy-class.md) of $N$ can be fixed by such a $g$. If the class of $n\ne1$ were fixed, $gng^{-1}=vnv^{-1}$ for some $v\in N$, so $v^{-1}g\notin N$ would centralize $n$, a contradiction. Conjugation by $g$ consequently fixes just the identity class. By [Brauer's permutation lemma](../../../../../../../brauer-s-permutation-lemma.md) it fixes just one [irreducible character](../../../../../../../irreducible-character.md), necessarily $1_N$.

For every nonprincipal $\varphi\in\operatorname{Irr}(N)$, its [inertia group of a character](../../../../../../../inertia-group-of-a-character.md) is therefore $I_G(\varphi)=N$. Since $N$ is normal, the restriction of the [induced character](../../../../../../../induced-character.md) is the sum of its conjugates, counted over $G/N$:

$$
(\varphi^G)_N=\sum_{gN\in G/N}\varphi^g.
$$

[Frobenius reciprocity](../../../../../../../frobenius-reciprocity.md) and [character orthogonality](../../../../../../../character-orthogonality.md) give

$$
\langle\varphi^G,\varphi^G\rangle_G
=\langle\varphi,(\varphi^G)_N\rangle_N
=|I_G(\varphi):N|=1.
$$

An actual [character](../../../../../../../character-of-a-representation.md) of norm one is irreducible. **Every nonprincipal [irreducible character](../../../../../../../irreducible-character.md) of $N$ therefore induces irreducibly to $G$.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
