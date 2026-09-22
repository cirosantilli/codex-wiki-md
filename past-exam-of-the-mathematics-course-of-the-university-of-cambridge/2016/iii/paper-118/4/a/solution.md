<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the usual additive [Čech cohomology](../../../../../../cech-cohomology.md) groups, $\mathcal F$ is understood to be a [sheaf of abelian groups](../../../../../../sheaf-of-abelian-groups.md). Order the index set of the [open cover](../../../../../../open-cover.md) $\mathfrak U=(U_i)$. The [Čech cochain group](../../../../../../cech-cochain-group.md) is

$$
\check C^q(\mathfrak U,\mathcal F)=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_q}),\qquad q\geq0.
$$

An empty intersection contributes the zero group. The [Čech coboundary](../../../../../../cech-coboundary.md) is the alternating sum of restriction maps:

$$
(\delta c)_{i_0\ldots i_{q+1}}
=\sum_{a=0}^{q+1}(-1)^a
c_{i_0\ldots\widehat{i_a}\ldots i_{q+1}}\big|_{U_{i_0}\cap\cdots\cap U_{i_{q+1}}}.
$$

Every double omission appears twice with opposite sign, so $\delta^2=0$. **The Čech cohomology is the cohomology of this cochain complex**:

$$
\boxed{\check H^q(\mathfrak U,\mathcal F)
=\frac{\ker(\delta:\check C^q\to\check C^{q+1})}{\operatorname{im}(\delta:\check C^{q-1}\to\check C^q)}.}
$$

Here $\check C^{-1}=0$. The [sheaf gluing axiom](../../../../../../sheaf-gluing-axiom.md) identifies $\check H^0(\mathfrak U,\mathcal F)$ with $\Gamma(X,\mathcal F)$. This definition is for the fixed cover; no limit over refinements is part of the group requested here. Without the abelian-group structure, this additive [Čech cochain complex](../../../../../../cech-cochain-complex.md) is not defined.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
