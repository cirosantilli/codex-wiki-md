# String with an endpoint mass

↑ **Parent:** [Wave equation on a string](wave-equation-on-a-string.md)

For a uniform string with [tension](tension.md) $T>0$, [linear mass density](linear-mass-density.md) $\rho>0$, left end fixed, and a freely transverse-moving point mass $M\geq0$ at $x=L$, the [wave equation](wave-equation-split.md) and endpoint law are

$$
\rho y_{tt}=Ty_{xx},\qquad y(0,t)=0,\qquad
M y_{tt}(L,t)=-Ty_x(L,t).
$$

The last equation is [Newton's second law](newton-s-second-law.md): the string pulls the mass back toward the interior, giving the minus sign. With [wave speed](wave-speed.md) $c=\sqrt{T/\rho}$, a nonzero [normal mode](normal-mode.md) has spatial part $X(x)=\sin(\omega x/c)$ and satisfies

$$
\cot\frac{\omega L}{c}=\frac{M\omega}{\rho c}.
$$

For $M>0$, its dimensionless roots $q=\omega L/c$ occur once in each $(n\pi,n\pi+\pi/2)$, $n\geq0$, because $\cot q$ decreases from infinity to zero while $Mq/(\rho L)$ increases. For $M=0$, $q=(n+1/2)\pi$: the right end has a homogeneous [Neumann boundary condition](neumann-boundary-condition.md). There is no nonzero zero-frequency mode, since a linear spatial profile vanishing at the left end and with zero right slope must vanish everywhere.

Multiplying the spatial equation by $X$ and using [integration by parts](integration-by-parts.md) gives

$$
\omega^2=\frac{T\int_0^L(X')^2\,dx}
{\rho\int_0^L X^2\,dx+M X(L)^2}>0.
$$

For two different modes, the same calculation gives the [weighted inner product](weighted-inner-product.md) orthogonality $\rho\int_0^L X_mX_n\,dx+M X_m(L)X_n(L)=0$. The endpoint mass therefore contributes to both inertia and mode orthogonality.

## ↑ Ancestors (7)

1. [Wave equation on a string](wave-equation-on-a-string.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/19/solution.md)
