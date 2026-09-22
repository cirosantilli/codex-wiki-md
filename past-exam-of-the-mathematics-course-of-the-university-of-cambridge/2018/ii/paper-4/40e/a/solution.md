<h1 id="40e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $y_r^{(E)}=y_{2r}$ and $y_r^{(O)}=y_{2r+1}$. Since $\omega_{2m}^2=\omega_m$,

$$
x_\ell=\sum_{r=0}^{m-1}\omega_m^{r\ell}y_{2r}
+\omega_{2m}^{\ell}\sum_{r=0}^{m-1}\omega_m^{r\ell}y_{2r+1}.
$$

Hence, for $0\leq\ell<m$, the [even--odd fast Fourier transform recursion](../../../../../../even-odd-fast-fourier-transform-recursion.md) is

$$
\boxed{x_\ell=x_\ell^{(E)}+\omega_{2m}^{\ell}x_\ell^{(O)},
\qquad
x_{\ell+m}=x_\ell^{(E)}-\omega_{2m}^{\ell}x_\ell^{(O)}}.
$$

Only one twiddle-factor multiplication is needed for each value of $\ell$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
