# Gamma impulse solution for linearly increasing diffusivity

↑ **Parent:** [Advection-diffusion equation](advection-diffusion-equation.md)

On $z>0$, consider $p_t+a p_z=D(zp_z)_z$ with $a,D>0$, zero scalar flux $ap-Dzp_z$ at the endpoints for $t>0$, and unit initial impulse at the origin. Put $r=a/D$ and $\eta=z/(Dt)$. The normalized [similarity solution](similarity-solution.md) is

$$
p(z,t)=\frac{\eta^r e^{-\eta}}{Dt\,\Gamma(1+r)}.
$$

The ansatz $p=(Dt)^{-1}f(\eta)$ gives $[\eta f'+(\eta-r)f]'=0$. Endpoint decay sets this integrated constant to zero and hence $f\propto\eta^re^{-\eta}$; the [gamma function](gamma-function.md) normalizes its [integral](integral.md) to one. Its scale is $Dt$, so it converges weakly to a unit impulse as $t\downarrow0$. Its [gamma distribution](gamma-distribution.md) shape is $1+r$, its maximum occurs at $z=at$, and its [expected value](expected-value.md) is $(a+D)t$. For width proportional to $z$, the associated [horizontally averaged plume concentration](horizontally-averaged-plume-concentration.md) is proportional to $z^{r-1}e^{-z/(Dt)}$: its interior maximum is $(a-D)t$ when $a>D$, its supremum occurs at the origin when $a=D$, and it is singular there when $0<a<D$. The physical finite source regularizes this ideal-origin behaviour.

## ↑ Ancestors (7)

1. [Advection-diffusion equation](advection-diffusion-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-345/2/solution.md)
