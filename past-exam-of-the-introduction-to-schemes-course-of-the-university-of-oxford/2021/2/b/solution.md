<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Discard empty members of the [open cover](../../../../open-cover.md): every [Čech cochain group](../../../../cech-cochain-group.md) factor supported on an empty intersection is the zero [abelian group](../../../../abelian-group.md), so this changes no [Čech cohomology](../../../../cech-cohomology.md). Every remaining member is the one-point space $X$; the index set is nonempty even if the same [open subset](../../../../open-set.md) is listed repeatedly. Choose a [well-order](../../../../well-order.md) with least index $\alpha$. Use the [ordered Čech cochain complex](../../../../ordered-cech-cochain-complex.md) permitted in the question:

$$
C^q=\prod_{i_0<\cdots<i_q} A,\qquad
(\delta s)_{i_0\cdots i_{q+1}}=\sum_{r=0}^{q+1}(-1)^r s_{i_0\cdots\widehat{i_r}\cdots i_{q+1}}.
$$

All restriction maps are identities. For $q\geq1$ define a [cochain homotopy](../../../../cochain-homotopy.md) $h_q:C^q\to C^{q-1}$ by

$$
(h_qs)_{i_0\cdots i_{q-1}}=
\begin{cases}
0,&i_0=\alpha,\\
s_{\alpha i_0\cdots i_{q-1}},&i_0>\alpha.
\end{cases}
$$

We verify $\delta h_q+h_{q+1}\delta=\operatorname{id}_{C^q}$ for every $q\geq1$. Fix $I=(i_0<\cdots<i_q)$. If $i_0=\alpha$, then $(h_{q+1}\delta s)_I=0$. In $(\delta h_qs)_I$, the term deleting $i_0$ is $s_I$ and every other term is zero because its retained first index is $\alpha$. Thus the identity holds on $I$.

If $i_0>\alpha$, then

$$
(\delta h_qs)_I=\sum_{r=0}^q(-1)^r s_{\alpha,I\setminus i_r},\qquad
(h_{q+1}\delta s)_I=(\delta s)_{\alpha,I}
=s_I-\sum_{r=0}^q(-1)^r s_{\alpha,I\setminus i_r}.
$$

Adding proves the identity in this case also. Each formula uses only finitely many terms on each component, so it remains valid for an infinite [open cover](../../../../open-cover.md) and arbitrary [abelian group](../../../../abelian-group.md) $A$.

If $s\in C^q$ is a [Čech cocycle](../../../../cech-cocycle-condition.md), then $\delta s=0$, and the identity gives $s=\delta(h_qs)$: every [Čech cocycle](../../../../cech-cocycle-condition.md) in positive degree is a [Čech coboundary](../../../../cech-coboundary.md). Therefore, using the permitted comparison with ordered [Čech cohomology](../../../../cech-cohomology.md),

$$
\boxed{\check H^q_{\mathcal U}(X,\underline A)=0\qquad(q\geq1).}
$$

The identity is asserted in positive degrees; degree zero has $H^0\cong A$, so an unaugmented contraction to zero in every degree would be incorrect.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
