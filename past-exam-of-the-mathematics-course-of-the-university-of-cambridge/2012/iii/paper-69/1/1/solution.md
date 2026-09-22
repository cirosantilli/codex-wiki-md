<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $I=(-1,1)$ and use the [clamped second-order Sobolev space](../../../../../../clamped-second-order-sobolev-space.md)

$$
H=H_0^2(I)=\{v\in H^2(I):v(\pm1)=v'(\pm1)=0\}.
$$

Here [weak derivatives](../../../../../../weak-derivative.md) up to order two are square integrable, with [Sobolev norm](../../../../../../sobolev-norm.md) $\|v\|_{H^2}^2=\|v\|_2^2+\|v'\|_2^2+\|v''\|_2^2$. The boundary values are the continuous traces given by the [Sobolev trace theorem](../../../../../../sobolev-trace-theorem.md), not arbitrary pointwise representatives. This space is the $H^2$ closure of $C_c^\infty(I)$, so it is a closed [Hilbert space](../../../../../../hilbert-space-split.md). The derivative boundary conditions are essential, and $H_0^1(I)$ alone is insufficient.

Define the symmetric [bilinear form](../../../../../../bilinear-form.md) and bounded linear functional

$$
a(u,v)=\int_I(pu''v''+qu'v'+ruv)\,dx,
\qquad \ell(v)=\int_I fv\,dx.
$$

Then the variational problem is

$$
\boxed{\min_{v\in H}J(v),\qquad
J(v)=\frac12\int_I\left(p(v'')^2+q(v')^2+rv^2\right)dx-\int_I fv\,dx.}
$$

For complex data replace $a$ by its sesquilinear version, take the real part of the forcing term and use absolute squares in $J$; the same argument applies.

Its first variation is $J'(u)[v]=a(u,v)-\ell(v)$. Thus stationary points satisfy $a(u,v)=\ell(v)$ for every $v\in H$, the [weak formulation of a clamped fourth-order equation](../../../../../../weak-formulation-of-a-clamped-fourth-order-equation.md). For smooth coefficients and functions, twice integrating the highest term and once the middle term gives the differential equation, with all boundary terms zero because $v=v'=0$ at both ends. With only the stated continuous coefficients, this manipulation is instead understood distributionally: compactly supported [test functions](../../../../../../test-function.md) give $(pu'')''-(qu')'+ru=f$ as a [distribution](../../../../../../distribution-mathematical-analysis.md). This avoids assuming nonexistent classical derivatives of $p$ or $q$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [1](../../1.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
