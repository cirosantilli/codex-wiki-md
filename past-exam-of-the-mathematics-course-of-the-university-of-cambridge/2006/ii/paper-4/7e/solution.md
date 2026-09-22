<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The nonzero [fixed point](../../../../../fixed-point.md) of the [logistic map](../../../../../logistic-map.md) is $x_*=(\mu-1)/\mu$, with multiplier $F'(x_*)=2-\mu$. It is stable for $1<\mu<3$, and its multiplier crosses $-1$ at $\mu=3$. To identify the emerging orbit explicitly, factor

$$
F^2(x)-x=-x(\mu x-\mu+1)
\left[\mu^2x^2-\mu(\mu+1)x+\mu+1\right].
$$

The remaining two roots, interchanged by $F$, are

$$
\boxed{x_{1,2}=\frac{\mu+1\pm\sqrt{(\mu+1)(\mu-3)}}{2\mu}}.
$$

They coincide with $x_*$ at three and are distinct for $\mu>3$. Their cycle multiplier is

$$
\Lambda_2=F'(x_1)F'(x_2)=\mu^2(1-2x_1)(1-2x_2)
=-\mu^2+2\mu+4.
$$

It lies between $-1$ and $1$ for $3<\mu<1+\sqrt6$. This establishes the first [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md) and the stable bifurcating two-cycle.

At $\mu_2=1+\sqrt6$, $\Lambda_2=-1$ and $d\Lambda_2/d\mu=-2\sqrt6\ne0$. The second flip is nondegenerate: for $H=F^2$ at either cycle point, the cubic flip coefficient is $c=(H'''/6)+(H''/2)^2=-\mathcal S H/6$ when $H'=-1$. Here $\mathcal S$ denotes the [Schwarzian derivative](../../../../../schwarzian-derivative.md). Since $\mathcal SF=-6/(1-2x)^2<0$ and $\mathcal S(F^2)=(\mathcal SF\circ F)(F')^2+\mathcal SF$, this coefficient is positive. Locally, after following the [fixed point](../../../../../fixed-point.md) of $H$, its second iterate has the form $H^2(y)-y=2a(\mu-\mu_2)y-2cy^3+\cdots$, with $a=2\sqrt6>0$. Nonzero roots therefore appear with $y^2\sim a(\mu-\mu_2)/c$ on the increasing-parameter side. These are a four-cycle of $F$, proving **the second [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md) occurs at $\mu=1+\sqrt6$**.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
