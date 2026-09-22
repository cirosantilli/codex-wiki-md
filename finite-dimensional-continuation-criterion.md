# Finite-dimensional continuation criterion

↑ **Parent:** [Picard-Lindelöf theorem](picard-lindelof-theorem.md)

Under the [Picard-Lindelöf theorem](picard-lindelof-theorem.md)'s hypotheses on $U\subset\mathbb R\times\mathbb R^d$, extend a [solution of a differential equation](solution-of-a-differential-equation.md) as far as possible, to a maximal [interval](interval-mathematics.md) $(T_-,T_+)$. If $T_+<\infty$, the time-state trajectory $(t,y(t))$ must eventually leave every [compact subset](compact-space.md) of $U$. Equivalently, confinement near $T_+$ to one [compact subset](compact-space.md) of $U$ permits continuation past $T_+$. See [Teschl, Section 2.6, Lemma 2.14 and Corollaries 2.15–2.16, pp. 52–53](https://www.mat.univie.ac.at/~gerald/ftp/book-ode/ode.pdf).

The domain restriction matters even for a bounded trajectory. Restrict $y'=1$, $y(0)=0$, to $U=\mathbb R\times(-1,1)$. Then $y(t)=t$ exists in this domain only for $-1<t<1$; at $t=1/2,3/4,9/10$ its values are $1/2,3/4,9/10$. As $t\uparrow1$, it approaches the excluded [boundary](boundary-of-a-set.md) point $(1,1)$ while remaining bounded. Its trajectory cannot fit into any [compact subset](compact-space.md) of $U$ near that endpoint. This is escape from a finite domain, without [finite-time blowup](finite-time-blowup.md) in norm. Enlarging the domain to $\mathbb R\times\mathbb R$ gives the same formula $y(t)=t$ for every real $t$.

Conversely, $y'=y$, $y(0)=1$, stays in the [compact set](compact-space.md) $[0,T]\times[1,e^T]$ for every fixed $T>0$. Its growing [exponential function](exponential-function.md) is unbounded over the entire future, but has no [finite-time blowup](finite-time-blowup.md). At $T=2$, its largest value on $[0,2]$ is only $e^2\approx7.38905610$. The relevant question is boundedness before each finite endpoint, rather than one bound valid forever. The [tangent function](tangent-function.md) in the diagram under the [Picard-Lindelöf theorem](picard-lindelof-theorem.md) illustrates the other possibility: its norm escapes every bound before $T=\pi/2$.

This criterion is useful because an estimate can secure continuation without an explicit formula. In a [finite-dimensional vector space](finite-dimensional-vector-space.md), a bounded [closed ball](closed-ball.md) is [compact](compact-space.md); a bounded state trajectory therefore supplies the needed [compact set](compact-space.md) when its time-state closure is inside the domain. That final proviso prevents mistaking a domain boundary for [finite-time blowup](finite-time-blowup.md).

A common sufficient estimate comes from global [Lipschitz continuity](lipschitz-continuity.md) in the state. Assume $U=I\times\mathbb R^d$ for an open time [interval](interval-mathematics.md) $I$, with $f$ continuous and a [Lipschitz constant](lipschitz-constant.md) $L\geq0$ valid for all states on each compact time [interval](interval-mathematics.md) under consideration. For $[t_0,T]\subset I$, let $B=\sup_{t_0\leq s\leq T}\|f(s,0)\|$, finite by [continuity](continuous-function.md). Then $\|f(t,y)\|\leq B+L\|y\|$, and the [Gronwall inequality](gronwall-inequality.md) gives, for $t_0\leq t\leq T$ wherever the solution already exists,

$$
\|y(t)\|\leq\begin{cases}\|y_0\|e^{L(t-t_0)}+\dfrac{B}{L}\bigl(e^{L(t-t_0)}-1\bigr),&L>0,\\\|y_0\|+B(t-t_0),&L=0.\end{cases}
$$

For instance, $y'=y+1$, $y(0)=0$, has $L=B=1$ and the exact solution $y(t)=e^t-1$, attaining this estimate; at $t=1$ the value is $e-1\approx1.71828183$. Finite bounds of this kind give continuation throughout $I$, with the analogous estimate backwards in time. When $I=\mathbb R$, this gives existence for all real times. If $I$ has a finite endpoint, it gives no continuation beyond that prescribed domain. The underlying linear-growth criterion is [Teschl, Theorem 2.17, p. 53](ordinary-differential-equations-and-dynamical-systems-by-gerald-teschl.md).

A brief explanation of the continuation mechanism suffices: within the protecting [compact set](compact-space.md), the [continuous function](continuous-function.md) $f$ is bounded, say by $M$. The [integral equation](integral-equation.md) yields $\|y(t)-y(s)\|\leq M|t-s|$ near the finite endpoint, so $y(t)$ has a limit $y_*$. The protecting [compact set](compact-space.md) puts $(T_+,y_*)$ inside $U$. Restarting the [initial value problem](initial-value-problem.md) there and using local uniqueness joins the trajectories.

## ↑ Ancestors (7)

1. [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Finite-time blowup](finite-time-blowup.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/25i/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-359/1/b/ii/solution.md)
- [Peano existence theorem](peano-existence-theorem.md)
- [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
