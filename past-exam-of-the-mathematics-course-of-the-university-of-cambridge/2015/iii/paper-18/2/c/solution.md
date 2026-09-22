<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove the [Bott-Chern Poincaré lemma](../../../../../../bott-chern-poincare-lemma.md) on a [polydisc](../../../../../../polydisc.md) $B$. Let $p,q\geq1$ and $d\alpha=0$, with $\alpha$ of type $(p,q)$. The allowed [Dolbeault-Poincaré lemma](../../../../../../dolbeault-poincare-lemma.md) first gives $\alpha=\bar\partial b_0$, where $b_0$ has type $(p,q-1)$. Since $\bar\partial\partial b_0=-\partial\alpha=0$, repeatedly applying the same lemma constructs

$$
b_j\in\mathcal A^{p+j,q-1-j}(B),\qquad
\bar\partial b_j=\partial b_{j-1}\quad(1\leq j\leq q-1).
$$

Zero spaces outside the allowed bidegrees cause no difficulty. The form $\partial b_{q-1}$ has type $(p+q,0)$, is holomorphic because its [Dolbeault operator](../../../../../../dolbeault-operator.md) vanishes, and is $\partial$-closed. The holomorphic [Poincaré lemma](../../../../../../poincare-lemma.md) on a [polydisc](../../../../../../polydisc.md) gives a holomorphic form $h$ of type $(p+q-1,0)$ with $\partial h=\partial b_{q-1}$. This holomorphic version follows from the radial homotopy formula: on positive-degree holomorphic forms the ordinary radial [Poincaré lemma](../../../../../../poincare-lemma.md) homotopy preserves holomorphic coefficients. If the displayed form is zero, take $h=0$.

Now $b_{q-1}-h$ is $\partial$-closed. The [conjugate Dolbeault-Poincaré lemma](../../../../../../conjugate-dolbeault-poincare-lemma.md), obtained by conjugating the allowed lemma, gives $b_{q-1}-h=\partial c_{q-1}$, since its holomorphic degree is positive. Moving backwards, if the last modified form is $\partial c_j$, then

$$
\partial(b_{j-1}+\bar\partial c_j)=0.
$$

Apply the [conjugate Dolbeault-Poincaré lemma](../../../../../../conjugate-dolbeault-poincare-lemma.md) again to obtain $b_{j-1}+\bar\partial c_j=\partial c_{j-1}$. The modification does not change its [Dolbeault operator](../../../../../../dolbeault-operator.md), so this process continues down to $b_0$. In the case $q=1$, subtract $h$ at this last step instead. Finally,

$$
\alpha=\bar\partial b_0=\bar\partial\partial c_0
=-\partial\bar\partial c_0.
$$

Thus **$\boxed{H^{p,q}_{BC}(B)=0\quad(p,q\geq1)}$**.

This vanishing fails on general [complex manifolds](../../../../../../complex-manifold.md). On the [complex projective line](../../../../../../complex-projective-line.md), let $\omega$ be its [Fubini-Study form](../../../../../../fubini-study-form.md). It is a $d$-closed $(1,1)$-form with $\int_{\mathbb P^1}\omega>0$. If it were $\partial\bar\partial f$, it would be the [exact differential form](../../../../../../exact-differential-form.md) $d(\bar\partial f)$, whose integral is zero by [Stokes theorem](../../../../../../stokes-theorem.md). Therefore **$\boxed{H^{1,1}_{BC}(\mathbb P^1)\ne0}$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
