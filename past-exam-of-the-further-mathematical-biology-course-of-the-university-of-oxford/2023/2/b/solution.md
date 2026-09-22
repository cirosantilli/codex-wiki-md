<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a consistency issue in the printed model. If $w\equiv w_0$ is imposed while retaining its evolution equation, then $0=\beta v-\gamma w_0$ forces $v\equiv\gamma w_0/\beta$. Thus the full two-equation system has no nonconstant [travelling wave](../../../../travelling-wave.md) with exactly constant $w$. Its constant solution exists only when $I=w_0-f(\gamma w_0/\beta)$. The intended wave calculation must treat the [recovery variable](../../../../recovery-variable.md) as externally frozen, leaving the scalar [reaction-diffusion equation](../../../../reaction-diffusion-system.md)

$$
v_t=Dv_{xx}+g(v),\qquad g(v)=f(v)+I-w_0.
$$

For this frozen-recovery reduction, let

$$
a_\pm=\frac{1+\alpha\pm\sqrt{1-\alpha+\alpha^2}}3.
$$

The [cubic polynomial](../../../../cubic-polynomial.md) $f$ has a local minimum at $a_-$ and a local maximum at $a_+$. Hence the condition

$$
\boxed{w_0-f(a_+)<I<w_0-f(a_-)}
$$

gives three distinct real roots $r_1<r_2<r_3$ of $g$, with

$$
g(v)=-(v-r_1)(v-r_2)(v-r_3).
$$

The outer roots are stable for the scalar spatially uniform dynamics and the middle root is unstable. Seek a [travelling wave](../../../../travelling-wave.md) $v(x,t)=V(z)$, where $z=x-ct$. The [travelling-wave reduction of a reaction-diffusion system](../../../../travelling-wave-reduction-of-a-reaction-diffusion-system.md) gives

$$
DV''+cV'-(V-r_1)(V-r_2)(V-r_3)=0.
$$

Let $\delta=r_3-r_1$ and choose

$$
V(z)=r_1+\frac{\delta}{1+\exp[\delta(z-z_0)/\sqrt{2D}]}.
$$

It has $V(-\infty)=r_3$, $V(+\infty)=r_1$ and

$$
V'=-\frac{(V-r_1)(r_3-V)}{\sqrt{2D}},\qquad
V''=\frac{(V-r_1)(r_3-V)(r_1+r_3-2V)}{2D}.
$$

Substitution leaves

$$
(V-r_1)(r_3-V)\left[\frac{r_1+r_3}{2}-r_2-\frac c{\sqrt{2D}}\right]=0.
$$

Consequently the [frozen-recovery cubic front](../../../../frozen-recovery-cubic-front.md) is

$$
\boxed{v(x,t)=r_1+\frac{r_3-r_1}{1+\exp\left[\frac{r_3-r_1}{\sqrt{2D}}(x-ct-z_0)\right]},\qquad
c=\sqrt{\frac D2}(r_1+r_3-2r_2).}
$$

Reflection $x\mapsto-x$ reverses the [front](../../../../front-solution.md) and its speed. A nonzero speed requires $r_2\ne(r_1+r_3)/2$; equality gives a stationary [front](../../../../front-solution.md) and is the [Maxwell balance for a scalar reaction-diffusion front](../../../../maxwell-balance-for-a-scalar-reaction-diffusion-front.md). Since the roots sum to $1+\alpha$, this stationary value is $I=w_0-f((1+\alpha)/3)$. For the simple admissible choice $I=w_0$, the roots are $0,\alpha,1$ and

$$
\boxed{V(z)=\frac1{1+e^{(z-z_0)/\sqrt{2D}}},\qquad c=\sqrt{\frac D2}(1-2\alpha).}
$$

This particular [front](../../../../front-solution.md) moves when $\alpha\ne1/2$. At $\alpha=1/2$, other currents inside the displayed open interval give moving [fronts](../../../../front-solution.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
