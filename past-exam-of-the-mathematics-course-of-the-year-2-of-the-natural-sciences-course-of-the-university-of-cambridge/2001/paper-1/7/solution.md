<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

**Boundary form.** For real [functions](../../../../function-split.md) and $\mathcal Ly=-(py')'+qy$, [integration by parts](../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\int_a^b(y_1\mathcal Ly_2-y_2\mathcal Ly_1)\,dx&=\int_a^b[-y_1(py_2')'+y_2(py_1')']\,dx\\
&=[p(y_2y_1'-y_1y_2')]_a^b.
\end{aligned}
$$

The integral terms containing $py_1'y_2'$ cancel, as do the $q$ terms. This is the [Lagrange identity for a Sturm-Liouville operator](../../../../lagrange-identity-for-a-sturm-liouville-operator.md). The [boundary conditions](../../../../boundary-condition.md) must make this boundary form zero for every admissible pair. Several suitable choices are homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) at both endpoints; homogeneous [Neumann boundary conditions](../../../../neumann-boundary-condition.md) at both endpoints; one of each; or separated homogeneous [Robin boundary conditions](../../../../robin-boundary-condition.md)

$$
\alpha_a y(a)+\beta_a p(a)y'(a)=0,\qquad\alpha_b y(b)+\beta_b p(b)y'(b)=0,
$$

where each fixed real pair $(\alpha,\beta)$ is nonzero. At each endpoint the two boundary data vectors are then proportional, making their antisymmetric product zero. Another choice is periodic data $y(a)=y(b)$ and $p(a)y'(a)=p(b)y'(b)$, which cancel the two endpoint contributions. These domains give the required [self-adjoint differential operator](../../../../self-adjoint-differential-operator.md) in the regular setting.

**Eigenfunctions.** Set $x=\cos\theta$, $0\leq\theta\leq\pi$, and $Y(\theta)=y(\cos\theta)$. The [chain rule](../../../../chain-rule.md) gives

$$
y'=-\frac{Y_\theta}{\sin\theta},\qquad(1-x^2)y''-xy'=Y_{\theta\theta}.
$$

The [Chebyshev differential equation](../../../../chebyshev-differential-equation.md) therefore becomes $Y''+n^2Y=0$, with $Y(0)=Y(\pi)=0$. For a positive integer $n$, the first condition excludes the cosine term and the second is satisfied by $\sin(n\theta)$. Thus

$$
\boxed{y_n(x)=N_n\sin(n\arccos x),\qquad\lambda_n=n^2,\qquad n=1,2,\ldots.}
$$

There is no nonzero $n=0$ [eigenfunction](../../../../eigenfunction.md): the transformed solution is linear in $\theta$ and vanishes at both endpoints only if identically zero. Negative $n$ merely repeats a positive mode with the opposite sign, so it is excluded from the indexing of an independent [eigenbasis](../../../../eigenbasis.md).

**Weight and normalization.** Multiplying the differential equation by $-1/\sqrt{1-x^2}$ puts it into [Sturm-Liouville form](../../../../sturm-liouville-form.md):

$$
-\frac d{dx}\left(\sqrt{1-x^2}\,y'\right)=\lambda\frac{y}{\sqrt{1-x^2}}.
$$

Hence $p=\sqrt{1-x^2}$, $q=0$ and $w=(1-x^2)^{-1/2}$. Under $x=\cos\theta$, the measure $w(x)\,dx$ becomes $-d\theta$, so

$$
\int_{-1}^1w(x)y_n(x)y_m(x)\,dx=N_nN_m\int_0^\pi\sin(n\theta)\sin(m\theta)\,d\theta=N_nN_m\frac\pi2\delta_{nm}.
$$

Therefore

$$
\boxed{w(x)=\frac1{\sqrt{1-x^2}},\qquad N_n=\sqrt{\frac2\pi}\quad(n\geq1).}
$$

These endpoints are singular because $p$ vanishes and $w$ diverges there, but the weight is integrable. Moreover $py_n'=-N_n n\cos(n\theta)$ remains finite, so the vanishing values of $y_n$ make the boundary form zero. These are the [Dirichlet eigenfunctions of the Chebyshev differential operator](../../../../dirichlet-eigenfunctions-of-the-chebyshev-differential-operator.md), not the first-kind [Chebyshev polynomials](../../../../chebyshev-polynomial.md) $\cos(n\arccos x)$, which have nonzero endpoint values.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
