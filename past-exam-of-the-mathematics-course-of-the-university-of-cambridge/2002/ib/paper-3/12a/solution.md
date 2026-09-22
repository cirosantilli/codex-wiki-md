<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

Use the weighted [inner product](../../../../../inner-product.md) $\langle u,v\rangle_r=\int_a^b r(x)u(x)v(x)\,dx$. For real [eigenfunctions](../../../../../eigenfunction.md), integration by parts with the zero endpoint values gives

$$
\int_a^b y_m\mathcal Ly_n\,dx
=\int_a^b[p y_m'y_n'+q y_my_n]dx
=\int_a^b y_n\mathcal Ly_m\,dx.
$$

Thus $(\lambda_n-\lambda_m)\langle y_m,y_n\rangle_r=0$. The regular separated [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) has simple [eigenvalues](../../../../../eigenvalue.md): for a fixed [eigenvalue](../../../../../eigenvalue.md), prescribing $y(a)=0$ leaves only the initial flux $p(a)y'(a)$ free, so uniqueness of the associated first-order system makes any two [eigenfunctions](../../../../../eigenfunction.md) proportional. Distinct [eigenfunctions](../../../../../eigenfunction.md) are therefore orthogonal, and choosing their signs and scales so that $\int r y_n^2=1$ gives

$$
\boxed{\langle y_m,y_n\rangle_r=\delta_{mn}}.
$$

The positive [energy](../../../../../energy.md) form $\int(p y'^2+q y^2)$ realizes $r^{-1}\mathcal L$ as a positive self-adjoint operator in this weighted space, with compact inverse on the bounded interval. The [spectral theorem for compact self-adjoint operators](../../../../../spectral-theorem-for-compact-hermitian-operators.md) supplies a complete eigenbasis. This is the standard regular [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md), also valid with continuous $p$ by working with the continuous flux $py'$.

For a source $F$, expand a zero-endpoint solution of $(\mathcal L-\mu r)y=F$ in that [basis](../../../../../basis.md). Multiplication by $y_n$ and unweighted integration give

$$
(\lambda_n-\mu)\langle y_n,y\rangle_r=\int_a^b y_n(\xi)F(\xi)\,d\xi.
$$

Since $\mu$ is not an [eigenvalue](../../../../../eigenvalue.md), every coefficient is determined. The [spectral Green function of a regular Sturm-Liouville problem](../../../../../spectral-green-function-of-a-regular-sturm-liouville-problem.md) is consequently

$$
\boxed{G_\mu(x,\xi)=\sum_{n=1}^\infty\frac{y_n(x)y_n(\xi)}{\lambda_n-\mu}}.
$$

Weighted completeness means $r(x)\sum_n y_n(x)y_n(\xi)=\delta(x-\xi)$ as a distribution, so applying $\mathcal L-\mu r$ to this series produces the required delta source. The source integration is with $d\xi$, explaining the absence of an additional factor $r(\xi)$ in the stated kernel.

For the subsequent operator $L=d^2/dx^2$ the sign is explicitly reversed: $y_n=\sqrt{2/\pi}\sin(nx)$ and $\lambda_n=-n^2$. To cover every real non-[eigenvalue](../../../../../eigenvalue.md) $\mu$, define the homogeneous solution

$$
S_\mu(x)=\begin{cases}\sinh(\sqrt\mu\,x)/\sqrt\mu,&\mu>0,\\x,&\mu=0,\\\sin(\sqrt{-\mu}\,x)/\sqrt{-\mu},&\mu<0.\end{cases}
$$

It satisfies $S_\mu(0)=0$, $S_\mu'(0)=1$ and $S_\mu''=\mu S_\mu$. Matching the two endpoint solutions continuously at $x=\xi$ with derivative jump $G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=1$ yields

$$
\boxed{G_\mu(x,\xi)=-\frac{S_\mu(x_<)S_\mu(\pi-x_>)}{S_\mu(\pi)},\qquad
x_<=\min(x,\xi),\quad x_>=\max(x,\xi)}.
$$

The denominator is nonzero precisely off the Dirichlet [eigenvalues](../../../../../eigenvalue.md) $\mu=-n^2$. In particular $G_0=-x_<(\pi-x_>)/\pi$. At $x=\xi=\pi/2$, its spectral expansion gives

$$
-\frac\pi4=-\frac2\pi\sum_{n=1}^\infty\frac{\sin^2(n\pi/2)}{n^2}
=-\frac2\pi\sum_{j=0}^\infty\frac1{(2j+1)^2}.
$$

This [odd reciprocal-square sum from a Dirichlet Green function](../../../../../odd-reciprocal-square-sum-from-a-dirichlet-green-function.md) proves $\boxed{\sum_{j=0}^\infty(2j+1)^{-2}=\pi^2/8}$.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
