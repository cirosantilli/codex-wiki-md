<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

The [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) of the [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md) is $m^2+m-2=(m-1)(m+2)=0$, giving the [homogeneous solution](../../../../../homogeneous-solution.md) $Ae^t+Be^{-2t}$. For the first forcing, a [particular solution](../../../../../particular-solution.md) of the form $Ce^{-t}$ gives $-2C=1$, so

$$
y=Ae^t+Be^{-2t}-\tfrac12e^{-t}.
$$

The [initial conditions](../../../../../initial-condition.md) impose $A+B=1/2$ and $A-2B=-1/2$, whence $A=1/6$, $B=1/3$. Thus **the first solution is**

$$
\boxed{y(t)=\tfrac16e^t+\tfrac13e^{-2t}-\tfrac12e^{-t}.}
$$

For the second forcing, $e^t$ is already a [homogeneous solution](../../../../../homogeneous-solution.md), so the usual exponential trial must be multiplied by $t$. Substitution of the [particular solution](../../../../../particular-solution.md) $Cte^t$ gives $3Ce^t=e^t$, hence $C=1/3$. Now $y=Ae^t+Be^{-2t}+te^t/3$, and the [initial conditions](../../../../../initial-condition.md) give $A+B=0$, $A-2B=-1/3$. Therefore **the resonant solution is**

$$
\boxed{y(t)=\left(\tfrac t3-\tfrac19\right)e^t+\tfrac19e^{-2t}.}
$$

The additional factor $t$ reflects [resonance in a differential equation](../../../../../resonance-in-a-differential-equation.md).

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
