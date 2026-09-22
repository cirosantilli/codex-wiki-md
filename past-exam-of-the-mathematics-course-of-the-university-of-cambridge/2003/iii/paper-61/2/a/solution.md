<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $E_k=e^{i(kx+k^3t)}$, $I=\int_L\varphi(l)\,d\lambda(l)$ and $A_k=\int_L\varphi(l)/(k+l)\,d\lambda(l)$. Introduce the dressing operator

$$
(\mathcal Fh)(k)=h(k)+iE_k\int_L\frac{h(l)}{k+l}\,d\lambda(l).
$$

The given [linear integral equation](../../../../../../linear-integral-equation.md) is $\mathcal F\varphi=E$, and $q=-I_x$. The appropriate contour and measure must permit differentiation under these integrals and avoid untreated kernel singularities.

For the specified spatial operator, direct differentiation gives

$$
M_kE_k=qE_k,\qquad
M_k(E_kA_k)=E_k(A_{k,xx}+ikA_{k,x}+qA_k).
$$

Inside the integral, replace $\varphi_{xx}(l)+q\varphi(l)$ by $M_l\varphi(l)+il\varphi_x(l)$. It follows that

$$
A_{k,xx}+ikA_{k,x}+qA_k
=\int_L\frac{M_l\varphi(l)}{k+l}\,d\lambda(l)+iI_x.
$$

Apply $M_k$ to $\varphi+iE_kA_k=E_k$. The last term contributes $-E_kI_x=qE_k$, canceling the right side, so

$$
\boxed{\mathcal F(M\varphi)=0.}
$$

This is precisely the homogeneous integral equation. Uniqueness of the original inhomogeneous solution implies a trivial homogeneous [null space](../../../../../../kernel-of-a-linear-map.md), hence $M\varphi=0$. This calculation is the spatial identity in [Cauchy-kernel dressing for the KdV equation](../../../../../../cauchy-kernel-dressing-for-the-kdv-equation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
