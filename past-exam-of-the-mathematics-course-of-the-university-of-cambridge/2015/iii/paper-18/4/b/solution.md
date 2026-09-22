<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Chern connection](../../../../../../chern-connection.md) decomposes on [vector-bundle-valued differential forms](../../../../../../vector-bundle-valued-differential-form.md) as $D=D'+D''$, where $D'=\nabla'_h$ raises holomorphic degree and $D''=\nabla''_h=\bar\partial_E$ raises antiholomorphic degree. In a [holomorphic local frame](../../../../../../holomorphic-local-trivialization.md), $D'=\partial+A\wedge$ and $D''=\bar\partial$. The type of the [curvature form of a connection](../../../../../../curvature-form.md) gives

$$
(D')^2=(D'')^2=0,\qquad D'D''+D''D'=F_h\wedge.
$$

The [Kähler metric](../../../../../../kahler-metric.md) and the [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) define the $L^2$ inner product and the [formal adjoints](../../../../../../formal-adjoint.md) $D'^*,D''^*$. The [Dolbeault Laplacians](../../../../../../dolbeault-laplacian.md) are

$$
\Delta'=D'D'^*+D'^*D',\qquad
\Delta''=D''D''^*+D''^*D''.
$$

Let $L=\omega\wedge$ be the [Lefschetz operator of a Kähler manifold](../../../../../../lefschetz-operator-of-a-kahler-manifold.md) and $\Lambda=L^*$ its [adjoint Lefschetz operator](../../../../../../adjoint-lefschetz-operator.md). With the ordinary commutator convention $[A,B]=AB-BA$, the printed [Kähler identities](../../../../../../kahler-identities.md) give

$$
D'^*=i[\Lambda,D''],\qquad D''^*=-i[\Lambda,D'].
$$

Substitution into the two [Dolbeault Laplacians](../../../../../../dolbeault-laplacian.md), followed by expansion, yields

$$
\begin{aligned}
\Delta''-\Delta'
&=-i\{D'', [\Lambda,D']\}-i\{D',[\Lambda,D'']\}\\
&=i[D'D''+D''D',\Lambda]\\
&=[iF_h\wedge,\Lambda].
\end{aligned}
$$

The middle line follows by cancelling the terms with $D'\Lambda D''$ and $D''\Lambda D'$; the remaining terms collect the anticommutator of the two differentials. Hence **$\boxed{\Delta''=\Delta'+[iF_h,\Lambda]}$**, where $iF_h$ denotes its wedge action. This is the [Bochner-Kodaira-Nakano identity](../../../../../../bochner-kodaira-nakano-identity.md) with the paper's sign convention.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
