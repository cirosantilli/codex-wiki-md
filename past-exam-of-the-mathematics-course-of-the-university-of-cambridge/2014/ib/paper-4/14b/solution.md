<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

For $\operatorname{Re}s>0$, integration by parts recursively in the [Laplace transform](../../../../../laplace-transform.md) gives

$$
 \boxed{\mathcal L[t^n](s)=\frac{n!}{s^{n+1}},\qquad
 \mathcal L[H(t-a)](s)=\int_a^\infty e^{-st}dt=\frac{e^{-as}}s.}
$$

The initial exponential boundary term vanishes, and $\mathcal L[1]=1/s$ starts the recursion. Here $H$ is the [Heaviside step function](../../../../../heaviside-step-function.md).

Transform the displacement in time, writing $Y(x,s)=\mathcal L_t[y](x,s)$. Zero initial displacement and velocity give $s^2Y=c^2Y_{xx}+g/s$. A particular solution is $g/s^3$, and the spatial homogeneous solutions are $e^{\pm sx/c}$. The prescribed far-field behavior excludes the growing exponential. The fixed boundary sets the remaining coefficient to $-g/s^3$, hence

$$
 Y(x,s)=\frac g{s^3}(1-e^{-sx/c}).
$$

Since $\mathcal L[t^2/2]=1/s^3$, the [Laplace transform time-shift rule](../../../../../laplace-transform-time-shift-rule.md) gives

$$
 \boxed{y(x,t)=\frac g2\left[t^2-H(t-x/c)(t-x/c)^2\right].}
$$

Equivalently, $y=gt^2/2$ for $t\leq x/c$, and $y=gxt/c-gx^2/(2c^2)$ for $t\geq x/c$. This solves the forced [wave equation](../../../../../wave-equation-split.md) in each region and has continuous displacement and first derivatives across the characteristic $t=x/c$, so it also solves the equation weakly there. It satisfies the fixed-end and initial conditions and equals $gt^2/2$ sufficiently far away at each fixed time. The end's influence travels at speed $c$.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
