<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

**Self-adjoint form.** Grouping the two derivative terms gives $[(1+\epsilon x)u']'-\epsilon u=-\lambda u$. Thus a regular [Sturm-Liouville operator](../../../../sturm-liouville-operator.md) is

$$
\boxed{\mathcal L=-\frac d{dx}\left[(1+\epsilon x)\frac d{dx}\right]+\epsilon,
\qquad p=1+\epsilon x,\quad q=\epsilon,\quad w=1.}
$$

The [boundary conditions](../../../../boundary-condition.md) are mixed [Neumann boundary conditions](../../../../neumann-boundary-condition.md) at zero and [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) at $\pi$. For $\epsilon\geq0$, $p>0$, $q\geq0$ and $w>0$, as required. The boundary term $[p(fg'-f'g)]_0^\pi$ vanishes for two functions satisfying these conditions, confirming self-adjointness on that domain.

**Constrained variation.** Introduce a [Lagrange multiplier](../../../../lagrange-multiplier.md) $\Lambda$ for the normalization and vary

$$
I[v]-\Lambda\left(\int_0^\pi wv^2\,dx-1\right).
$$

Its first variation is

$$
2[pv'\delta v]_0^\pi+2\int_0^\pi[-(pv')'+qv-\Lambda wv]\delta v\,dx.
$$

The endpoint term vanishes because $v'(0)=0$ and $\delta v(\pi)=0$. The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is therefore

$$
-(pv')'+qv=\Lambda wv,
$$

which is exactly the original [eigenvalue](../../../../eigenvalue.md) problem for the boxed choices of $p,q,w$. Multiply by $v$ and integrate by parts. The same endpoint conditions give

$$
I[v]=\int_0^\pi(pv'^2+qv^2)\,dx=\Lambda\int_0^\pi wv^2\,dx=\Lambda.
$$

Thus **the stationary functional values are the [eigenvalues](../../../../eigenvalue.md)**, with $\Lambda=\lambda$. More generally, before normalization the relevant [Rayleigh quotient](../../../../rayleigh-quotient.md) is

$$
\mathcal R_\epsilon[v]=\frac{\int_0^\pi[(1+\epsilon x)v'^2+\epsilon v^2]dx}{\int_0^\pi v^2dx}.
$$

**Unperturbed ground mode.** At $\epsilon=0$, the equation is $-u''=\lambda u$. The quadratic form is nonnegative, and zero [eigenvalue](../../../../eigenvalue.md) would force a constant function incompatible with the endpoint at $\pi$. For positive $\lambda$, $u=A\cos(\sqrt\lambda x)+B\sin(\sqrt\lambda x)$. The derivative condition forces $B=0$, while the other endpoint gives $\cos(\pi\sqrt\lambda)=0$. Hence

$$
\lambda_n=(n+1/2)^2,\qquad n=0,1,2,\ldots.
$$

The lowest [eigenvalue](../../../../eigenvalue.md) and normalized [eigenfunction](../../../../eigenfunction.md) are

$$
\boxed{\lambda_0=\frac14,\qquad U_0(x)=\sqrt{\frac2\pi}\cos\frac x2,\qquad
\int_0^\pi U_0^2dx=1.}
$$

**Trial-function bound.** The [Rayleigh-Ritz method](../../../../rayleigh-ritz-method.md) says that the minimum [eigenvalue](../../../../eigenvalue.md) is no larger than the quotient of any admissible trial function. The same $U_0$ still satisfies both [boundary conditions](../../../../boundary-condition.md) and retains unit norm. Its derivative is $U_0'=-\sqrt{2/\pi}\sin(x/2)/2$, giving

$$
\mathcal R_\epsilon[U_0]=\frac14+\epsilon\left[1+\frac1{2\pi}\int_0^\pi x\sin^2\frac x2\,dx\right].
$$

Using $\sin^2(x/2)=(1-\cos x)/2$,

$$
\int_0^\pi x\sin^2\frac x2\,dx=\frac{\pi^2}{4}+1.
$$

Therefore the [affine-parameter Sturm-Liouville eigenvalue bound](../../../../affine-parameter-sturm-liouville-eigenvalue-bound.md) is

$$
\boxed{\lambda_{\min}(\epsilon)\leq\frac14+\epsilon\left(1+\frac\pi8+\frac1{2\pi}\right)
\simeq\frac14+1.551854\epsilon.}
$$

This is an upper bound for every $\epsilon\geq0$, not merely a small-parameter approximation. As a lower-bound check, $p\geq1$ and the unperturbed variational minimum imply $\mathcal R_\epsilon[v]\geq1/4+\epsilon$ for every admissible normalized $v$. Thus

$$
\boxed{\frac14+\epsilon\leq\lambda_{\min}(\epsilon)\leq\frac14+\left(1+\frac\pi8+\frac1{2\pi}\right)\epsilon.}
$$

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2017](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
