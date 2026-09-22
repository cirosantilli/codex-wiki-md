<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use

$$
(\mathcal Fg)(\mathbf q)=\int_{\mathbb R^3}
g(\mathbf r)e^{-i\mathbf q\cdot\mathbf r}d\mathbf r,
\qquad
\mathcal F^{-1}h=\frac1{(2\pi)^3}\int h(\mathbf q)e^{i\mathbf q\cdot\mathbf r}d\mathbf q.
$$

The [adjoint operator](../../../../../../adjoint-operator.md) is consequently

$$
\boxed{\mathcal F^*=(2\pi)^3\mathcal F^{-1}.}
$$

With a unitary Fourier normalization, this is simply $\mathcal F^*=\mathcal F^{-1}$.

At fixed incident direction and wavenumber, define

$$
(TV)(\widehat{\mathbf r})
=-\frac1{4\pi}\int_D
e^{-ik_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)\cdot\mathbf r}
V(\mathbf r)d\mathbf r.
$$

Taking the complex conjugate of the kernel gives

$$
\boxed{
(T^*g)(\mathbf r)
=-\frac1{4\pi}\int_{S^2}
e^{ik_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)\cdot\mathbf r}
g(\widehat{\mathbf r})dS(\widehat{\mathbf r}),
\qquad \mathbf r\in D.}
$$

The least-squares minimizer of $\|TV-f_\infty\|^2$ satisfies the [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) $T^*TV=T^*f_\infty$. Fourier inversion on the measured transfer-vector set is exactly the corresponding Moore--Penrose reconstruction $T^\dagger f_\infty$; hence the formal solution in part (i) is the minimum-norm least-squares solution when the data are incomplete or inconsistent.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
