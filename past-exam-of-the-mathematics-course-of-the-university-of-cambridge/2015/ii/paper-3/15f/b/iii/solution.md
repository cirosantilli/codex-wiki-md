<h1 id="15f/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**As printed, the equivalence needs a transitivity hypothesis.** A group acting trivially on two points has $\mathbb C\Omega=\mathbb C_G\oplus\mathbb C_G$, so $V$ is one-dimensional and irreducible, although the action is not even transitive.

Here is the intended result for a transitive action. The set is then finite, and, for a point stabilizer $H$, its [permutation character](../../../../../../../permutation-character.md) is $\chi=\operatorname{Ind}_H^G1$. [Frobenius reciprocity](../../../../../../../frobenius-reciprocity.md) gives

$$
\langle\chi,\chi\rangle_G=\langle1,\operatorname{Res}_H^G\chi\rangle_H=\#\{H\hbox{-orbits on }\Omega\}.
$$

The last equality follows because an $H$-fixed vector has constant coefficients on each orbit. There is exactly one trivial constituent, since the action is transitive. Therefore, writing $\chi=1+\psi$ for the character of $V$,

$$
\langle\psi,\psi\rangle_G=\#\{H\hbox{-orbits on }\Omega\}-1.
$$

By [character orthogonality](../../../../../../../character-orthogonality.md), $V$ is [irreducible](../../../../../../../irreducible-representation.md) exactly when this equals $1$. One stabilizer orbit is $\{\omega\}$, so this happens exactly when $H$ is transitive on $\Omega\setminus\{\omega\}$, equivalently when $G$ is [two-transitive](../../../../../../../two-transitive-group-action.md). Moreover $V$ is not trivial, since a transitive action has only one independent fixed vector in the whole permutation module.

The complete correction without assuming transitivity is also precise: **$V$ is irreducible exactly for a two-transitive action or the exceptional action on two fixed points**. Indeed for a finite set with $r$ orbits, the fixed subspace of $V$ has dimension $r-1$. If $r>1$ and $V$ is irreducible, $V$ must itself be a one-dimensional trivial module, forcing $|\Omega|=2$ and $r=2$. If $\Omega$ is infinite, $V$ is infinite-dimensional and cannot be irreducible: any nonzero vector generates a submodule of dimension at most $|G|$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [15F](../../../15f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
