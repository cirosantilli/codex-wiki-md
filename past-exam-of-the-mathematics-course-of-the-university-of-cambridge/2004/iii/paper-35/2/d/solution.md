<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [power-wealth investment with running utility](../../../../../../power-wealth-investment-with-running-utility.md) objective is homogeneous of degree $\gamma$ in wealth: scaling both wealth and positions by $a>0$ scales the reward by $a^\gamma$. Accordingly set $J(w,t)=A(t)w^\gamma$. Then

$$
\frac{J_w}{J_{ww}}=\frac{w}{\gamma-1},\qquad
\boxed{\frac{B^*}{w}=1-\frac{\mu-r}{(1-\gamma)\sigma^2},\qquad\frac{\pi^*}{w}=\frac{\mu-r}{(1-\gamma)\sigma^2}.}
$$

For completeness the remaining equation is $A'+\kappa A+e^{-\rho t}=0$, $A(T)=1$, where

$$
\kappa=\gamma r+\frac{\gamma(\mu-r)^2}{2(1-\gamma)\sigma^2},\qquad
A(t)=e^{\kappa(T-t)}+\int_t^T e^{\kappa(s-t)-\rho s}ds>0.
$$

This confirms $J_{ww}<0$. The constant optimal risky fraction also makes wealth a positive [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) when started positive.

Financially the [relative risk aversion coefficient](../../../../../../relative-risk-aversion-coefficient.md) is $1-\gamma$. Increasing $\gamma$ reduces [risk aversion](../../../../../../risk-aversion.md), raises the risky fraction, and decreases the bond fraction: its derivative is $-(\mu-r)/[\sigma^2(1-\gamma)^2]<0$. If the risky fraction is below one, some wealth is lent; at one, none is invested in bonds; above one, $B^*<0$ represents borrowing to leverage the risky position. As $\gamma\uparrow1$ the risky fraction becomes unbounded, consistent with the absence of a finite unconstrained optimum for linear utility and positive excess drift. As $\gamma\downarrow0$ the limiting fraction is $(\mu-r)/\sigma^2$, the logarithmic-utility allocation obtained by the appropriately rescaled power-utility limit; the literal objective at $\gamma=0$ would be constant and would not select a unique strategy.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
