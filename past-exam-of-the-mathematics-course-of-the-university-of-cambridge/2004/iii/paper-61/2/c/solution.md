<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Identical oriented [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) imply a rotation-invariant solution whenever the Dirichlet problem is unique. For $\lambda\geq0$, uniqueness follows directly: the difference $h$ of two solutions has zero boundary trace, and [integration by parts](../../../../../../integration-by-parts.md) gives $\int_D|\nabla h|^2+4\lambda\int_D|h|^2=0$. Thus $h=0$. The same conclusion holds for a nonresonant negative parameter by invertibility of the [Dirichlet Laplacian](../../../../../../dirichlet-laplacian.md) shift. Then $q(az)=q(z)$, all three normal traces equal a common $q_N(s)$, and $\Psi_j=\Psi$.

Set

$$
e(k)=e^{\ell(k+\lambda/k)/2},\qquad\Phi(k)=\int_{-\ell/2}^{\ell/2}e^{(k+\lambda/k)s}\left[\frac12 f'(s)+\frac\lambda kf(s)\right]ds.
$$

Divide the global relation by $E(-iak)$. Using $1+a+\bar a=0$ yields $E(-ik)/E(-iak)=e(\bar ak)$ and $E(-i\bar ak)/E(-iak)=e(-k)$. Hence

$$
\boxed{e(\bar ak)\Psi(k)+e(-k)\Psi(\bar ak)+\Psi(ak)=2iA(k),}
$$

where the requested known function is

$$
\boxed{A(k)=e(\bar ak)\Phi(k)+e(-k)\Phi(\bar ak)+\Phi(ak).}
$$

For an explicitly derivative-free form, put $H(k)=\int_{-\ell/2}^{\ell/2}e^{(k+\lambda/k)s}f(s)ds$ and $f_*=f(-\ell/2)=f(\ell/2)$. An [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\Phi(k)=f_*\sinh\!\left(\frac\ell2(k+\lambda/k)\right)-\frac12\left(k-\frac\lambda k\right)H(k).
$$

The uniqueness qualification cannot be removed for every real $\lambda$: at a [Dirichlet Laplacian eigenvalue](../../../../../../dirichlet-laplacian-eigenvalue.md) a homogeneous addition need not preserve rotation invariance. The scalar reduced relation then applies to the rotation-averaged solution, but not necessarily to the originally chosen solution. Part (d) treats this genuine exceptional case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
