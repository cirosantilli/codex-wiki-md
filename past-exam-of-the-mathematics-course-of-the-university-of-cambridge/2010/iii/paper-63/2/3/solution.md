<h1 id="2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the differential expression as $Lu=(pu'')''+qu$, with a suitable differential-operator domain and the stated clamped boundary conditions. For sufficiently smooth $u,v$ in that domain, twice integrating by parts gives

$$
\langle Lu,v\rangle
=\left[(pu'')'\overline v-pu''\overline{v'}\right]_{-1}^{1}
+\int_{-1}^{1}\left(pu''\overline{v''}+qu\overline v\right)dx
=\int_{-1}^{1}\left(pu''\overline{v''}+qu\overline v\right)dx.
$$

The boundary term vanishes because $v=v'=0$ at both ends. For real coefficients this form is symmetric/Hermitian. In particular

$$
\boxed{\langle Lu,u\rangle=\int_{-1}^{1}\left(p|u''|^2+q|u|^2\right)dx>0\quad(u\ne0).}
$$

Indeed nonnegativity follows from $p>0$ and $q\ge0$. If the integral were zero, $u''=0$ almost everywhere in the interval, so $u$ would be affine. Its endpoint values then force $u=0$. This proves strict positivity on the intended clamped domain and gives the [weak formulation of a clamped fourth-order equation](../../../../../../weak-formulation-of-a-clamped-fourth-order-equation.md).

There is a genuine domain issue in the literal wording. The closure of clamped smooth functions in the stated [L2 norm](../../../../../../l2-norm.md) is all of $L^2(-1,1)$, since it contains the dense set $C_c^\infty(-1,1)$. Boundary traces are not retained by that closure, and a fourth-order expression does not define an operator on every element of $L^2$. For example $p=(1-x^2)^2$, $q=0$ satisfy the given sign conditions, but $u=\mathbf1_{(-1/2,1/2)}$ belongs to this closure and makes $(pu'')''$ a distribution rather than an $L^2$ function. Even a general twice-smooth function need not have the four derivatives required by the classical expression.

A rigorous classical repair is to take smooth enough coefficients, for example $p\in C^2([-1,1])$, $q\in C([-1,1])$, and use a clamped domain such as $H^4\cap H_0^2$ in $L^2$, with the appropriate operator realization. A weak repair uses the [clamped second-order Sobolev space](../../../../../../clamped-second-order-sobolev-space.md) $H_0^2$ and the form just displayed, with hypotheses ensuring its boundedness and closure; uniform positivity $p\ge p_0>0$ makes it coercive there. The integration-by-parts and strict-positivity proof does not need that stronger uniform bound, but existence and completion statements must not be inferred from the original $L^2$ closure alone. The printed $L[f]$ with an expression in $u$ is also a harmless variable-name mismatch; the calculation consistently uses $Lu$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2](../../2.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
