<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $l>0$ and use the [inner product](../../../../../inner-product-split.md) $\langle u,v\rangle=\int_0^l\overline u v\,dx$ on the [Hilbert space](../../../../../hilbert-space-split.md) $L^2(0,l)$. The [differential operator](../../../../../differential-operator.md) has domain

$$
D(\mathcal L)=\{u\in H^2(0,l):u(0)=u(l)=0\},
$$

where $H^2$ is a [Sobolev space](../../../../../sobolev-space-split.md). Twice applying [integration by parts](../../../../../integration-by-parts.md) gives the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md)

$$
\langle u,\mathcal Lv\rangle-\langle\mathcal Lu,v\rangle
=[\overline u v'-\overline{u'}v]_0^l.
$$

The [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) make this expression zero for $u,v\in D(\mathcal L)$, and the [formal adjoint](../../../../../formal-adjoint.md) is $\mathcal L^*=d^2/dx^2+1$. To obtain the domain of the [adjoint operator](../../../../../adjoint-operator.md), initially impose the [boundary conditions](../../../../../boundary-condition.md) only on $u$. The remaining expression is $-[\overline{u'}v]_0^l$. Since $u'(0)$ and $u'(l)$ vary independently, it vanishes for all such $u$ exactly when $v(0)=v(l)=0$. The adjoint domain is therefore the original domain: this is full [self-adjointness](../../../../../self-adjoint-operator.md), including the [boundary conditions](../../../../../boundary-condition.md).

Consequently the [eigenvalues](../../../../../eigenvalue.md) are real, [eigenfunctions](../../../../../eigenfunction.md) for distinct [eigenvalues](../../../../../eigenvalue.md) are [orthogonal](../../../../../orthogonal-vectors.md), and regular [Sturm-Liouville theory](../../../../../sturm-liouville-theory-split.md) supplies a complete [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md). Here these objects can be exhibited explicitly:

$$
\boxed{\phi_n(x)=\sqrt{\frac2l}\sin\frac{n\pi x}{l},\qquad
\lambda_n=1-\left(\frac{n\pi}{l}\right)^2,\qquad n=1,2,\ldots.}
$$

Indeed $\mathcal L\phi_n=\lambda_n\phi_n$, and the [Fourier sine basis](../../../../../fourier-sine-basis.md) is complete in $L^2(0,l)$. There are no additional [eigenvalues](../../../../../eigenvalue.md): for a nonzero [eigenfunction](../../../../../eigenfunction.md) $u$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\lambda=1-\frac{\int_0^l|u'|^2\,dx}{\int_0^l|u|^2\,dx}<1,
$$

so $u''+(1-\lambda)u=0$ and the endpoint values force $\sqrt{1-\lambda}\,l=n\pi$. All these [eigenvalues](../../../../../eigenvalue.md) are simple. The [eigenvectors](../../../../../eigenvector.md) are precisely the nonzero multiples of these [eigenfunctions](../../../../../eigenfunction.md), regarded as [vectors](../../../../../vector.md) in the [Hilbert space](../../../../../hilbert-space-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
