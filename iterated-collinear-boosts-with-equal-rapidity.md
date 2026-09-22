# Iterated collinear boosts with equal rapidity

↑ **Parent:** [Rapidity](rapidity.md)

Starting from rest, compose $n$ positive collinear [Lorentz boosts](lorentz-boost.md), each with the same finite [rapidity](rapidity.md) $\alpha>0$. Each step has relative [velocity](velocity.md) $w=c\tanh\alpha$, measured in the preceding rest [inertial frame](inertial-frame.md). The [relativistic velocity-addition formula](velocity-addition-formula.md) gives

$$
u_0=0,\qquad u_{n+1}=\frac{u_n+w}{1+u_nw/c^2},\qquad \theta_n=n\alpha,\qquad u_n=c\tanh(n\alpha).
$$

These are equal increments of [rapidity](rapidity.md), not equal increments of [velocity](velocity.md) measured in the original [inertial frame](inertial-frame.md). They can describe a chain of relatively moving [inertial frames](inertial-frame.md) or successive idealized changes of a massive particle's motion; no particular acceleration schedule is assumed. [David Tong, General Relativity, §1.2.4: collinear boost composition and rapidity](https://davidtong.org/teaching/general-relativity/grhtml/S1).

For a relative [velocity](velocity.md) $w=c/2$ at each step,

$$
\alpha=\operatorname{artanh}(1/2)=\frac12\ln3,\qquad \frac{u_n}{c}=\frac{3^n-1}{3^n+1}.
$$

The first four [velocities](velocity.md) are $u_0=0$, $u_1=c/2$, $u_2=4c/5$, and $u_3=13c/14$. At step eight, $u_8/c=3280/3281\approx0.99969521$. The [rapidities](rapidity.md) grow by the same amount at each step, while the successive [velocity](velocity.md) increments become smaller.

<a id="image-rapidity-collinear-boosts"></a>
![](rapidity-collinear-boosts.png)

**[Figure 6](#image-rapidity-collinear-boosts). Equal collinear boosts add rapidities linearly while their composed velocities approach the speed of light**. The illustrative sequence uses relative [velocity](velocity.md) $c/2$ per step and $n=0,\ldots,8$. The horizontal coordinate counts boosts, rather than elapsed time. The line at $u_n/c=1$ marks the [speed of light](speed-of-light.md); every plotted [velocity](velocity.md) is strictly below it.

A short derivation applies the [hyperbolic-function identity](hyperbolic-function-identity.md) for $\tanh(a+b)$ to the recurrence, giving $\theta_{n+1}=\theta_n+\alpha$. Substituting $\tanh x=(e^{2x}-1)/(e^{2x}+1)$ and $e^{2\alpha}=3$ gives the displayed closed expression. In particular,

$$
1-\frac{u_n}{c}=\frac{2}{3^n+1}>0
$$

for every finite nonnegative integer $n$. The [limit](limit-of-a-function.md) is $u_n\to c$ as $n\to\infty$, but no finite sequence reaches the [speed of light](speed-of-light.md). This illustrates the beauty of [rapidity](rapidity.md): unbounded additive parameters coexist with bounded physical [velocities](velocity.md). Replacing every step by a negative [rapidity](rapidity.md) gives the corresponding approach to $-c$.

## ↑ Ancestors (7)

1. [Rapidity](rapidity.md)
2. [Lorentz boost](lorentz-boost.md)
3. [Lorentz transformation](lorentz-transformation.md)
4. [Special relativity](special-relativity-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4/4b/solution.md)
- [Rapidity](rapidity.md)
