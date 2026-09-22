# Green kernels for a radial dipole Euler equation

↑ **Parent:** [Green's function](green-s-function-split.md)

The homogeneous [Cauchy-Euler equation](cauchy-euler-equation.md) $Ly=0$ has fundamental solutions $x,x^{-1}$ on $x>0$, with [Wronskian](wronskian.md) $-2/x$. Requiring decay at both endpoints gives the unweighted [Green's function](green-s-function-split.md)

$$
G_D(x,\xi)=\begin{cases}-x/2,&x\leq\xi,\\-\xi^2/(2x),&x\geq\xi.\end{cases}
$$

Requiring zero initial value and derivative at zero instead gives the forward kernel

$$
G_0(x,\xi)=\begin{cases}0,&x\leq\xi,\\(x-\xi^2/x)/2,&x\geq\xi.\end{cases}
$$

Both kernels are continuous and have first-derivative jump one at $x=\xi$, so $L_xG=\delta(x-\xi)$. Away from that point they solve the homogeneous equation. Integrating against the forcing with ordinary measure $d\xi$ yields the respective solutions whenever the integral and endpoint limits converge. Their difference is $G_0-G_D=x/2$, independent of $\xi$, so the solutions differ by the homogeneous term $(x/2)\int f(\xi)d\xi$ for integrable forcing. For example, the two choices for an indicator forcing on $(0,1)$ differ by $x/2$. Specifying a differential operator without its endpoint conditions does not specify its Green kernel.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/3/solution.md)
