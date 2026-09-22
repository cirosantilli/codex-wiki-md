<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Order the index set of the [open cover](../../../../../../open-cover.md) $\mathcal U=(U_i)$. For the [sheaf of abelian groups](../../../../../../sheaf-of-abelian-groups.md) $\mathcal F$, the [Čech cochain group](../../../../../../cech-cochain-group.md) is

$$
C^p(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_p}
\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p}).
$$

It is a product, not a finite-support sum. The [Čech coboundary](../../../../../../cech-coboundary.md) is

$$
(\delta c)_{i_0\ldots i_{p+1}}
=\sum_{j=0}^{p+1}(-1)^j
c_{i_0\ldots\widehat{i_j}\ldots i_{p+1}}\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

Every term in $\delta^2c$ occurs twice with opposite signs, so $\delta^2=0$. The [Čech cohomology](../../../../../../cech-cohomology.md) of the cover is $\check H^p(\mathcal U,\mathcal F)=\ker\delta/\operatorname{im}\delta$. Refinements induce maps on these groups; different choices of refinement indices give maps related by a [cochain homotopy](../../../../../../cochain-homotopy.md), hence the same map on [cohomology](../../../../../../cohomology-split.md). Taking the [direct limit](../../../../../../direct-limit-of-abelian-groups.md) over covers gives

$$
\boxed{\check H^p(X,\mathcal F)=\varinjlim_{\mathcal U}\check H^p(\mathcal U,\mathcal F).}
$$

One may use locally finite covers, since a [complex manifold](../../../../../../complex-manifold.md) is a [paracompact space](../../../../../../paracompact-space.md) and these covers are cofinal. In degree zero this recovers the group of global sections by the [sheaf](../../../../../../sheaf-mathematics.md) gluing axiom.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
