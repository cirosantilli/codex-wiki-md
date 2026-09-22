<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [exterior derivative](../../../../../exterior-derivative.md) is an $\mathbb R$-linear map $d:\Omega^p(M)\to\Omega^{p+1}(M)$, agrees with the differential $df$ of a [smooth function](../../../../../smooth-function.md), satisfies the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) $d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^p\alpha\wedge d\beta$ for $\alpha\in\Omega^p(M)$, and has $d^2=0$. These properties determine it locally and hence globally. To see locality directly, if a [differential form](../../../../../differential-form-split.md) $\alpha$ vanishes near $x$, choose a [smooth bump function](../../../../../smooth-bump-function.md) $\chi$ equal to one near $x$ and supported where $\alpha=0$. The identity $d(\chi\alpha)=d\chi\wedge\alpha+\chi d\alpha$ gives $(d\alpha)_x=0$. Thus global forms can be computed using local extensions in a [manifold chart](../../../../../manifold-chart.md).

In coordinates write $\alpha=\sum_Ia_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_p}$. Since $d(dx^i)=d^2x^i=0$, the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) forces

$$
d\alpha=\sum_{I,j}\partial_ja_I\,dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_p}.
$$

This is the [uniqueness of the exterior derivative from its axioms](../../../../../uniqueness-of-the-exterior-derivative-from-its-axioms.md). The coordinate formula also establishes existence: it has the stated properties, and the [chain rule](../../../../../chain-rule.md) shows that coordinate changes give the same operator.

The [de Rham cohomology](../../../../../de-rham-cohomology.md) is the real [quotient vector space](../../../../../quotient-vector-space.md)

$$
H^p_{\mathrm{dR}}(M)=\frac{\ker(d:\Omega^p(M)\to\Omega^{p+1}(M))}{\operatorname{im}(d:\Omega^{p-1}(M)\to\Omega^p(M))}.
$$

Thus a [cohomology class](../../../../../cohomology-class.md) records a [closed differential form](../../../../../closed-differential-form.md) modulo an [exact differential form](../../../../../exact-differential-form.md). In degree zero there are no exact forms; closed functions are locally constant. The [Poincaré lemma](../../../../../poincare-lemma.md) says that every closed form of positive degree on a star-shaped open subset of $\mathbb R^n$ is exact, and hence that positive-degree closed forms are locally exact on a [smooth manifold](../../../../../smooth-manifold.md).

For the [first de Rham cohomology of the two-sphere](../../../../../first-de-rham-cohomology-of-the-two-sphere.md), let $U=S^2\setminus\{N\}$ and $V=S^2\setminus\{S\}$. [Stereographic projection](../../../../../stereographic-projection.md) identifies each with $\mathbb R^2$, so a closed one-form $\alpha$ has primitives $f_U,f_V$. On the connected overlap $U\cap V$, the [derivative](../../../../../derivative.md) of $f_U-f_V$ is zero, so this difference is a constant. Subtracting that constant from $f_U$ makes the primitives agree. They glue to a global smooth primitive. Therefore **$H^1_{\mathrm{dR}}(S^2)=0$.**

Let $q:S^2\to\mathbb{RP}^2$ be the double [covering map](../../../../../covering-space.md) and $a$ the [antipodal map](../../../../../antipodal-map.md). The [pullback of a differential form](../../../../../pullback-of-a-differential-form.md) identifies forms downstairs with $a$-invariant forms upstairs. Averaging $(\eta+a^*\eta)/2$ commutes with $d$. If an invariant form is exact upstairs, averaging its primitive proves it exact downstairs. Conversely an invariant [cohomology class](../../../../../cohomology-class.md) has an invariant representative by the same averaging. This proves the [de Rham cohomology of a finite quotient](../../../../../de-rham-cohomology-of-a-finite-quotient.md) identification $H^p_{\mathrm{dR}}(\mathbb{RP}^2)\cong H^p_{\mathrm{dR}}(S^2)^{a^*}$. In degree zero the sphere is connected and $a^*$ fixes constants; degree one is zero; in degree two the granted action is multiplication by $-1$, whose invariant real subspace is zero. Forms of degree greater than two vanish. Hence

$$
\boxed{H^p_{\mathrm{dR}}(\mathbb{RP}^2)=\begin{cases}\mathbb R,&p=0,\\0,&p>0.\end{cases}}
$$

This is real [de Rham cohomology](../../../../../de-rham-cohomology.md); it does not detect the integral two-torsion of the [real projective plane](../../../../../real-projective-plane.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
