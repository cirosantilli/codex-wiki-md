<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A smooth [differential form](../../../../../../differential-form-split.md) of degree $p$ is a smooth section of $\Lambda^pT^*M$, so

$$
\Omega^p(M)=\Gamma(\Lambda^pT^*M).
$$

It is equivalently a smooth alternating covariant $p$-tensor field. In a [coordinate chart](../../../../../../manifold-chart.md) $x^1,\ldots,x^n$ it has a unique expression

$$
\omega=\sum_{i_1<\cdots<i_p}a_{i_1\cdots i_p}\,dx^{i_1}\wedge\cdots\wedge dx^{i_p}
$$

with smooth coefficients. At $p=0$ these are the [smooth functions](../../../../../../smooth-function.md), and for $p>n$ the space is zero.

Define the [exterior derivative](../../../../../../exterior-derivative.md) in a chart by

$$
d\omega=\sum_{I,j}\frac{\partial a_I}{\partial x^j}\,dx^j\wedge dx^I.
$$

To check that it is well-defined, let $y^1,\ldots,y^n$ be other smooth coordinates. The expression $dy^a=\sum_i(\partial_i y^a)dx^i$ satisfies

$$
d_x(dy^a)=\sum_{i,j}(\partial_j\partial_i y^a)\,dx^j\wedge dx^i=0
$$

because the coefficients are symmetric and the wedge products antisymmetric. The coordinate formula also satisfies the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md), and for a function $b$ the [chain rule](../../../../../../chain-rule.md) gives $d_xb=\sum_a(\partial b/\partial y^a)dy^a=d_yb$. Applying these two facts to $\omega=\sum_I b_I\,dy^I$ yields $d_x\omega=\sum_I d_yb_I\wedge dy^I=d_y\omega$. Thus the local operators agree on overlaps and define a global [linear map](../../../../../../linear-map.md) $d:\Omega^p(M)\to\Omega^{p+1}(M)$.

A second application in any chart gives

$$
d^2\omega=\sum_{I,j,k}(\partial_k\partial_j a_I)\,dx^k\wedge dx^j\wedge dx^I=0,
$$

again by symmetry of mixed derivatives and antisymmetry of the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md). Consequently every [exact differential form](../../../../../../exact-differential-form.md) is closed. Put $\Omega^{-1}(M)=0$ and define the [de Rham cohomology](../../../../../../de-rham-cohomology.md) by

$$
\boxed{H^p_{\mathrm{dR}}(M)=\frac{\ker(d:\Omega^p\to\Omega^{p+1})}{\operatorname{im}(d:\Omega^{p-1}\to\Omega^p)}.}
$$

The identity $d^2=0$ is exactly what puts the denominator inside the numerator, making this quotient meaningful. Since $\Omega^p(M)=0$ for $p>\dim M$, **$H^p_{\mathrm{dR}}(M)=0$ in those degrees**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
