<h1 id="29k/solution">Solution</h1>

↑ **Parent:** [29K](../29k.md)

Assume a finite optimum with $X>0$ and continuous price near its completion time. With [costate](../../../../../costate.md) $p^*$ for the remaining-file state, the minimization [Hamiltonian of an optimal-control problem](../../../../../hamiltonian-of-an-optimal-control-problem.md) is $H=u(p(t)-p^*)$. It is independent of $x$, so $p^*$ is constant. By the [Pontryagin maximum principle](../../../../../pontryagin-maximum-principle.md), pointwise minimization over $[0,1]$ gives

$$
\boxed{u(t)=1\text{ if }p(t)<p^*,\qquad u(t)=0\text{ if }p(t)>p^*.}
$$

This is a [bang-bang control](../../../../../bang-bang-control.md) away from equality. At equality partial transmission or either endpoint rate is allowed. This also follows by exchanging a small amount of transmission from a more expensive time to a cheaper unused time. The [free-terminal-time transversality condition](../../../../../free-terminal-time-transversality-condition.md) is $\min_uH(T,u)+2\gamma T=0$. Since $T>0$, it forces $p^*>p(T)$ and terminal transmission at rate one, yielding

$$
\boxed{p^*=p(T)+2\gamma T.}
$$

Without regularity/existence hypotheses an arbitrary known price need not have a finite differentiable optimum; the equality is the interior terminal-time condition used here.

For $p(t)=t+1/t$, $X=1$, feasible completion requires $T>1$ for finite cost. The price decreases to its minimum at one and then increases. Its cheapest unrestricted interval of length one has endpoints $a,a+1$ of equal price, giving $a(a+1)=1$ and $a+1=\varphi=(1+\sqrt5)/2$. For $1<T\leq\varphi$, the cheapest length-one subset of $[0,T]$ is the terminal interval $[T-1,T]$: its left endpoint has at least the price of its right endpoint, and the earlier times are still more expensive. For $T\geq\varphi$ the transmission minimum is unchanged from that unrestricted interval, while the delay cost increases, so no optimum lies beyond $\varphi$.

For the terminal-interval policy the total cost is

$$
J(T)=T-\frac12+\log\frac T{T-1}+\gamma T^2,\qquad
J'(T)=1-\frac1{T(T-1)}+2\gamma T.
$$

Its [derivative](../../../../../derivative.md) is strictly increasing on $T>1$, since $J''(T)=(2T-1)/[T^2(T-1)^2]+2\gamma>0$. It is negative near one and positive at $\varphi$, so the unique global optimum is

$$
\boxed{u=1\text{ on }[T-1,T],\quad u=0\text{ earlier},\qquad\frac1{(T-1)T}=1+2\gamma T.}
$$

There is exactly one [positive root](../../../../../positive-root.md): none lies in $(0,1)$ because the left side is negative, and the strictly monotone comparison gives exactly one in $(1,\varphi)$. Its threshold is $p(T-1)=p(T)+2\gamma T$.

## ↑ Ancestors (10)

1. [29K](../29k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
