# Weak focus at the Hopf threshold of a basal activator-inhibitor model

↑ **Parent:** [Basally forced quadratic activator-inhibitor model](basally-forced-quadratic-activator-inhibitor-model.md)

At $q=a=(r-1)/(r+1)>0$, the reaction [eigenvalues](eigenvalue.md) are $\pm i\sqrt a$. This linear marginal case is a weakly attracting focus, not a nonlinear center. To check it directly, put $u=(1+r)(1+x)$, $v=(1+r)^2(1+y)$, $h=(1+a)/2$, $\beta=(1-a)/2$, $\omega=\sqrt a$, and $X=x$, $Y=(hy-a x)/\omega$. The equations become $\dot X=-\omega Y+F_2+F_3+O(4)$, $\dot Y=\omega X+G_2+G_3+O(4)$, with

$$
F_2=(\beta X-\omega Y)^2/h,\quad F_3=-(aX+\omega Y)(\beta X-\omega Y)^2/h^2,\quad G_2=\omega(hX^2-F_2),\quad G_3=-\omega F_3.
$$

On the [unit circle](complex-unit-circle.md) write $A=\cos\theta F_2+\sin\theta G_2$, $B=\cos\theta F_3+\sin\theta G_3$, $C=\cos\theta G_2-\sin\theta F_2$. In [polar coordinates](polar-coordinates.md), $d\varrho/d\theta=(A/\omega)\varrho^2+(B/\omega-AC/\omega^2)\varrho^3+O(\varrho^4)$. The quadratic angular average vanishes. Integrating the quadratic correction over a whole cycle contributes its final squared integral, also zero, leaving the cubic average. Using the even trigonometric moments gives $\langle B\rangle=a/4$ and $\langle AC\rangle/\omega=(a+1)/8$. The [Poincaré map](poincare-map.md) is therefore $\varrho\mapsto\varrho+[2\pi/\omega](a-1)\varrho^3/8+O(\varrho^4)$. Since $0<a<1$, it contracts sufficiently small positive radii and proves nonlinear [asymptotic stability](asymptotic-stability.md) at the threshold.

## ↑ Ancestors (8)

1. [Basally forced quadratic activator-inhibitor model](basally-forced-quadratic-activator-inhibitor-model.md)
2. [Reaction–diffusion system](reaction-diffusion-system.md)
3. [Diffusion equation](diffusion-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75/1/solution.md)
