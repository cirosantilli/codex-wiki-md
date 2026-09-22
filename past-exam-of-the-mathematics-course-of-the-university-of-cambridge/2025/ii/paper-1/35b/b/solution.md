<h1 id="35b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
q=\frac{im\lambda}{\hbar^2k},\qquad r=e^{ika},\qquad
\boldsymbol\Psi=\begin{pmatrix}\psi(-a)\\\psi(0)\\\psi(a)\end{pmatrix}.
$$

The [integral](../../../../../../integral.md) equation becomes

$$
\psi(x)=e^{ikx}+q\left\{e^{ik|x+a|}\psi(-a)+e^{ik|x|}\psi(0)+e^{ik|x-a|}\psi(a)\right\}.
$$

Evaluating it at the three delta [functions](../../../../../../function-split.md) gives

$$
\begin{aligned}
\psi(-a)&=r^{-1}+q\{\psi(-a)+r\psi(0)+r^2\psi(a)\},\\
\psi(0)&=1+q\{r\psi(-a)+\psi(0)+r\psi(a)\},\\
\psi(a)&=r+q\{r^2\psi(-a)+r\psi(0)+\psi(a)\}.
\end{aligned}
$$

Thus

$$
\left[I-q\begin{pmatrix}1&r&r^2\\r&1&r\\r^2&r&1\end{pmatrix}\right]
\boldsymbol\Psi
=\begin{pmatrix}r^{-1}\\1\\r\end{pmatrix}.
$$

For $x>a$, all three Green-function terms are proportional to $e^{ikx}$. Hence

$$
S_{++}(k)=1+q\left\{r\psi(-a)+\psi(0)+r^{-1}\psi(a)\right\}.
$$

Now define $\gamma=ik\hbar^2/(\lambda m)$, so that $q=-1/\gamma$. If $M$ denotes the [matrix](../../../../../../matrix.md) multiplying $\boldsymbol\Psi$, direct evaluation gives

$$
\det M=\frac{r^4}{\gamma^3}\left[1-\gamma-2r^{-2}(1+\gamma)+r^{-4}(1+\gamma)^3\right].
$$

The displayed algebraic equation is therefore exactly the condition that the finite-dimensional scattering system become singular. Its solutions are poles of the analytically continued [scattering amplitude](../../../../../../scattering-amplitude.md).

To see the imaginary-axis poles directly, write $k=i\kappa$ with $\kappa>0$. When $a\to0$, the equation reduces to

$$
\gamma^2(\gamma+3)=0,
$$

and its nonzero root is $\gamma=-3$, or

$$
\kappa=\frac{3m\lambda}{\hbar^2}.
$$

This is the [bound state](../../../../../../bound-state.md) of the coincident potential $-3\lambda\delta(x)$. When $a\to\infty$, the three centres decouple and the roots approach

$$
\gamma=-1,\qquad \kappa=\frac{m\lambda}{\hbar^2},
$$

with exponentially small splitting. A pole at $k=i\kappa$ has energy $E=-\hbar^2\kappa^2/(2m)$ and an exponentially decaying [wavefunction](../../../../../../wave-function.md), so these upper imaginary-axis singularities represent [bound states](../../../../../../bound-state.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [35B](../../35b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
