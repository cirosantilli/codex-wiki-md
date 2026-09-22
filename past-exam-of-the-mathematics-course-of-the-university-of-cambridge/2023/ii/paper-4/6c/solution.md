<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Put $a=f'(0)>0$. Linearizing the [morphogen reaction-diffusion equation](../../../../../morphogen-reaction-diffusion-equation.md) at $C=0$ gives

$$
C_t=DC_{xx}+aC.
$$

Seek separated modes $C(x,t)=X(x)e^{\lambda t}$. Then

$$
DX''+aX=\lambda X,
\qquad
X(0)=0,\quad X'(L)=0.
$$

The [mixed Dirichlet-Neumann modes on an interval](../../../../../mixed-dirichlet-neumann-modes-on-an-interval.md) are

$$
X_n(x)=\sin(k_nx),
\qquad
k_n=\frac{(n+1/2)\pi}{L},
\qquad n=0,1,2,\ldots.
$$

Indeed, the Dirichlet condition selects sine functions, while the Neumann condition requires $\cos(k_nL)=0$. Their growth rates are

$$
\lambda_n=a-Dk_n^2
=a-D\frac{(n+1/2)^2\pi^2}{L^2}.
$$

The largest growth rate is the lowest mode,

$$
\lambda_0=a-\frac{D\pi^2}{4L^2}.
$$

Linear stability requires $\lambda_0<0$, after which all higher modes also decay. Therefore the [critical length for a linearly growing morphogen](../../../../../critical-length-for-a-linearly-growing-morphogen.md) is

$$
\boxed{
L<\frac\pi2\sqrt{\frac{D}{f'(0)}}.}
$$

Equality gives a neutral lowest mode, while a larger domain is linearly unstable.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
