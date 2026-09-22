<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The space of smooth [differential forms](../../../../../../differential-form-split.md) of degree $p$ is

$$
\boxed{\Omega^p(M)=\Gamma(\Lambda^pT^*M).}
$$

Thus a form assigns smoothly to each point an alternating $p$-linear function on its [tangent space](../../../../../../tangent-space.md). Here $\Omega^0(M)=C^\infty(M)$, and forms of degree greater than $\dim M$ vanish. The [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) gives the graded [exterior algebra](../../../../../../exterior-algebra.md) of forms.

The [exterior derivative](../../../../../../exterior-derivative.md) is an $\mathbb R$-linear map of degree one satisfying the following axioms: $df(X)=X(f)$ for functions; for a $p$-form $\alpha$,

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^p\alpha\wedge d\beta;
$$

and $d^2=0$. The sign is the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md).

To construct it, write in a [coordinate chart](../../../../../../manifold-chart.md)

$$
\alpha=\sum_{i_1<\cdots<i_p}a_{i_1\ldots i_p}\,
dx^{i_1}\wedge\cdots\wedge dx^{i_p},
\qquad
d\alpha=\sum_{i_1<\cdots<i_p}da_{i_1\ldots i_p}\wedge
dx^{i_1}\wedge\cdots\wedge dx^{i_p}.
$$

This formula is linear, agrees with differentiation on functions and obeys the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md). Its square vanishes because symmetric second partial derivatives are contracted against antisymmetric wedge products.

The construction is independent of the chart. For coordinates $y^j=y^j(x)$, the [chain rule](../../../../../../chain-rule.md) gives $dy^j=\sum_i(\partial_i y^j)dx^i$, and the coordinate formula gives $d(dy^j)=0$ by equality of mixed partial derivatives. Consequently, expressing a form as $\sum_I b_I\,dy^I$ and applying the $x$-coordinate formula gives exactly $\sum_I db_I\wedge dy^I$, the $y$-coordinate formula. The local constructions agree on overlaps and therefore define a global [exterior derivative](../../../../../../exterior-derivative.md).

For uniqueness, first derive locality from the axioms. If $\alpha$ vanishes near $p$, choose a [smooth bump function](../../../../../../smooth-bump-function.md) $\chi$ supported in that neighborhood and equal to one near $p$. Then $\chi\alpha=0$, and

$$
0=d(\chi\alpha)=d\chi\wedge\alpha+\chi\,d\alpha
$$

implies $(d\alpha)_p=0$. Thus the value depends only on the local germ of $\alpha$. Local coordinate functions can be extended using bump functions, so the same axioms apply to their germs. Since $d(dx^i)=d^2x^i=0$, the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md) forces precisely the coordinate formula above. **The exterior derivative exists and is unique**, as expressed by [uniqueness of the exterior derivative from its axioms](../../../../../../uniqueness-of-the-exterior-derivative-from-its-axioms.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
