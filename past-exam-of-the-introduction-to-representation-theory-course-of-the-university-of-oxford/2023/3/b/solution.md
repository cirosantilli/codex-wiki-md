<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the [complex vector space](../../../../complex-vector-space.md) $\operatorname{CF}(G)$ of [class functions](../../../../class-function.md), define the [linear operator](../../../../linear-operator.md)

$$
Tf(g)=f(g^{-1}).
$$

This is a complex-[linear map](../../../../linear-map.md) and satisfies $T^2=I$. It is well-defined on [class functions](../../../../class-function.md), because [inversion of conjugacy classes](../../../../inversion-of-conjugacy-classes.md) takes an entire [conjugacy class](../../../../conjugacy-class.md) $K$ to another [conjugacy class](../../../../conjugacy-class.md) $K^{-1}$.

Use first the [basis](../../../../basis.md) consisting of the [indicator functions](../../../../indicator-function.md) $1_K$ of the [conjugacy classes](../../../../conjugacy-class.md). The [linear operator](../../../../linear-operator.md) $T$ permutes this [basis](../../../../basis.md) by $1_K\mapsto1_{K^{-1}}$. A [permutation matrix](../../../../permutation-matrix.md) has [trace](../../../../matrix-trace.md) equal to the number of fixed [basis vectors](../../../../basis-vector.md), so

$$
\operatorname{tr}T=\#\{K:K=K^{-1}\}.
$$

The right-hand side counts the [real conjugacy classes](../../../../real-conjugacy-class.md).

By [character orthogonality](../../../../character-orthogonality.md) and completeness, the [irreducible characters](../../../../irreducible-character.md) are another [basis](../../../../basis.md) of $\operatorname{CF}(G)$. Part (a) gives $T\chi=\overline\chi$. The pointwise [complex conjugate](../../../../complex-conjugate.md) of an [irreducible character](../../../../irreducible-character.md) is again an [irreducible character](../../../../irreducible-character.md): conjugate the representing [matrices](../../../../matrix.md), and conjugate any hypothetical proper [invariant subspace](../../../../invariant-subspace.md) back to contradict irreducibility. Thus $T$ also permutes this [basis](../../../../basis.md), and

$$
\operatorname{tr}T=\#\{\chi\in\operatorname{Irr}(G):\chi=\overline\chi\}.
$$

Here $\chi=\overline\chi$ means exactly that $\chi$ is a [real-valued character](../../../../real-valued-character.md). Equality of the [trace](../../../../matrix-trace.md) in these two [bases](../../../../basis.md) proves

$$
\boxed{\#\{\text{real-valued irreducible characters}\}
=\#\{\text{real conjugacy classes}\}.}
$$

This is the [real character and real conjugacy class counting theorem](../../../../real-character-and-real-conjugacy-class-counting-theorem.md). The [linear operator](../../../../linear-operator.md) used in the proof is $f\mapsto f\circ\operatorname{inv}$; on the [irreducible character](../../../../irreducible-character.md) [basis](../../../../basis.md) it agrees with pointwise [complex conjugation](../../../../complex-conjugation.md), although pointwise [complex conjugation](../../../../complex-conjugation.md) itself is not a complex-[linear map](../../../../linear-map.md) on all [class functions](../../../../class-function.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
