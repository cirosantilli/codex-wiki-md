<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

Set $y=a^2$. Multiplication of the [Friedmann equation](../../../../../friedmann-equations.md) by $4a^4$ gives

$$
\dot y^2=4\Gamma-4y+\frac{4\Lambda}{3}y^2.
$$

For the expanding branch emerging from $y(0)=0$, **$\dot y(0)=2\sqrt\Gamma$**. Differentiating where $\dot y\ne0$ gives $\ddot y=(4\Lambda/3)y-2$, and continuity extends it through a regular turning point. Put $\kappa=\sqrt{4\Lambda/3}$. Solving this linear equation with both initial data gives

$$
\boxed{a^2(t)=\frac3{2\Lambda}\left[1-\cosh\kappa t+\lambda\sinh\kappa t\right],\qquad
\lambda=2\sqrt{\frac{\Lambda\Gamma}{3}}}.
$$

Initially $a(t)\sim(2\sqrt\Gamma\,t)^{1/2}$. If $\lambda>1$, $y$ stays positive and strictly increasing; at late times $a\sim[3(\lambda-1)/(4\Lambda)]^{1/2}e^{\kappa t/2}$. This universe expands forever.

If $0<\lambda<1$, expansion stops when $\tanh\kappa t_{\max}=\lambda$, giving

$$
\boxed{t_{\max}=\kappa^{-1}\operatorname{artanh}\lambda,\quad
a_{\max}^2=\frac3{2\Lambda}(1-\sqrt{1-\lambda^2}),\quad
t_{\rm crunch}=2t_{\max}}.
$$

The physical solution expands from zero and then symmetrically recollapses to zero; negative $a^2$ beyond this interval is not a continuation of a real scale factor.

<a id="12c/image-scale-factor-histories-for-closed-radiation-universes-with-positive-cosmological-constant-eternal-expansion-for-lambda-above-one-and-finite-time-recollapse-for-lambda-below-one"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1-radiation-universes.png)

**[Figure 2](#12c/image-scale-factor-histories-for-closed-radiation-universes-with-positive-cosmological-constant-eternal-expansion-for-lambda-above-one-and-finite-time-recollapse-for-lambda-below-one). Scale-factor histories for closed radiation universes with positive cosmological constant: eternal expansion for lambda above one and finite-time recollapse for lambda below one**.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
