<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h=\Delta x$, $k=\Delta t$, and assume $a,u$ are sufficiently [smooth](../../../../../../smooth-function.md) for the following [Taylor expansions](../../../../../../taylor-expansion.md). The [symmetric half-grid diffusion consistency](../../../../../../symmetric-half-grid-diffusion-consistency.md) calculation gives

$$
L_hu=\frac{a(x-h/2)[u(x-h)-u(x)]+a(x+h/2)[u(x+h)-u(x)]}{h^2}=(au_x)_x+h^2E_2+O(h^4),
$$

where

$$
E_2=\frac{a u_{xxxx}}{12}+\frac{a'u_{xxx}}6+\frac{a''u_{xx}}8+\frac{a'''u_x}{24}.
$$

The [normalized local truncation error](../../../../../../normalized-local-truncation-error.md) of the full update is consequently

$$
\mathcal T_{h,k}=\frac{u(x,t+k)-u(x,t)}k-L_hu=u_t-(au_x)_x+\frac{k}{2}u_{tt}-h^2E_2+O(k^2+h^4).
$$

**The PDF prints an [advection equation](../../../../../../transport-equation.md), $u_t=a(x)u_x$, whereas this stencil approximates conservative diffusion, $u_t=(au_x)_x$.** For the literal printed equation the leading defect is $(a-a')u_x-a u_{xx}$, which generally does not vanish: the method is **inconsistent, with an $O(1)$ normalized defect**.

For the intended [variable-coefficient conservative diffusion equation](../../../../../../variable-coefficient-conservative-diffusion-equation.md), the first two terms cancel and $\mathcal T_{h,k}=O(k+h^2)$. Under the parabolic step scaling $k=O(h^2)$, this is **$O(h^2)$**, while the unnormalized one-step [local truncation error](../../../../../../local-truncation-error.md) is $k\mathcal T_{h,k}=O(h^4)$. These two orders use different normalizations. With [numerical stability](../../../../../../stability-of-a-numerical-method.md) and compatible smooth initial and [boundary conditions](../../../../../../boundary-condition.md), the intended diffusion problem has global error $O(k+h^2)$ on a fixed time interval. Positivity and boundedness of $a$ alone do not justify the displayed [Taylor expansion](../../../../../../taylor-expansion.md); coefficient regularity is also needed for that error formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
