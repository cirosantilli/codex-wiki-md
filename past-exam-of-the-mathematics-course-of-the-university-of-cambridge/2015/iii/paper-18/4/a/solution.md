<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Chern connection](../../../../../../chern-connection.md) of a [Hermitian metric on a holomorphic vector bundle](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) is the unique [connection on a vector bundle](../../../../../../connection-vector-bundle.md) compatible with that metric and whose $(0,1)$ part is the bundle's [Dolbeault operator](../../../../../../dolbeault-operator.md) $\bar\partial_E$. Fix a [holomorphic local frame](../../../../../../holomorphic-local-trivialization.md) and column coefficients for sections. Write the metric as $h(s,t)=\bar s^T Ht$, conjugate-linear in the first argument, and write the connection as $Ds=ds+A s$. The condition $D^{0,1}=\bar\partial_E$ forces $A$ to have type $(1,0)$. [Metric compatibility](../../../../../../metric-compatibility.md) requires

$$
dH=A^\dagger H+HA,
$$

where the dagger conjugates the differential-form coefficients as well as transposing the matrix. Taking the $(1,0)$ part gives **$\boxed{A=H^{-1}\partial H}$**. Its conjugate-transpose supplies the $(0,1)$ metric equation because $H$ is Hermitian. This proves uniqueness and local existence.

Under a holomorphic change of frame $e'=eg$, the metric matrix becomes $H'=g^\dagger Hg$. The [local formula for the Chern connection on a vector bundle](../../../../../../local-formula-for-the-chern-connection-on-a-vector-bundle.md) then gives

$$
A'=g^{-1}Ag+g^{-1}\partial g.
$$

This is precisely the transformation rule for a [connection on a vector bundle](../../../../../../connection-vector-bundle.md), so the local connections glue and establish global existence. No Kähler hypothesis is needed for this part.

Extend $D$ to [vector-bundle-valued differential forms](../../../../../../vector-bundle-valued-differential-form.md) by the graded Leibniz rule. The [curvature form of a connection](../../../../../../curvature-form.md) is the tensorial square $F_h=D^2$, acting by exterior multiplication. In the chosen frame,

$$
F_h=dA+A\wedge A=\bar\partial(H^{-1}\partial H).
$$

Indeed $\partial A+A\wedge A=0$ by differentiating $H^{-1}H=I$. It follows that $F_h$ has type $(1,1)$; the gauge change is $F'_h=g^{-1}F_hg$. Thus it is a global smooth two-form with values in $\operatorname{End}(E)$, namely an element of $\mathcal A^2(\operatorname{End}(E))$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
