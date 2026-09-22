<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Engquist-Osher method](../../../../../engquist-osher-method.md) is an upwind [finite volume method](../../../../../finite-volume-method.md). For cell values $U_j^n$, mesh width $h$ and time step $k$, put $r=k/h$ and use the conservative update

$$
U_j^{n+1}=U_j^n-r\bigl[F(U_j^n,U_{j+1}^n)-F(U_{j-1}^n,U_j^n)\bigr],
$$

where the [numerical flux](../../../../../numerical-flux.md) is

$$
\boxed{F(a,b)=f(0)+\int_0^a\max\{f'(s),0\}ds+\int_0^b\min\{f'(s),0\}ds.}
$$

[Consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) follows from $F(u,u)=f(u)$. Positive [characteristic speeds](../../../../../characteristic-speed.md) use the left state, and negative speeds use the right state. The flux difference telescopes when summed over cells, giving a discrete [conservation law](../../../../../conservation-law.md). The method is first order in space and time for smooth solutions; its [conservation law](../../../../../conservation-law.md) form is also appropriate when [shock waves](../../../../../shock-wave.md) develop.

Let $s_*$ be the unique [sonic point of a scalar flux](../../../../../sonic-point-of-a-scalar-flux.md), $f'(s_*)=0$. [Convexity](../../../../../convex-function.md) implies $f'<0$ to its left and $f'>0$ to its right. Put $f_*=f(s_*)$ and split

$$
f^+(u)=\begin{cases}0&u\le s_*,\\f(u)-f_*&u>s_*,\end{cases}
\qquad f^-(u)=\begin{cases}f(u)-f_*&u<s_*,\\0&u\ge s_* .\end{cases}
$$

Then $f=f_*+f^++f^-$, $(f^+)'\ge0$, $(f^-)'\le0$, and

$$
F(a,b)=f_*+f^+(a)+f^-(b).
$$

This is the [sonic-point splitting of a convex Engquist-Osher flux](../../../../../sonic-point-splitting-of-a-convex-engquist-osher-flux.md). If both states are above $s_*$, $F=f(a)$; if both are below it, $F=f(b)$. Across a transsonic [rarefaction wave](../../../../../rarefaction-wave.md), $a\le s_*\le b$, the flux is the minimum $f_*$. In the opposite crossing it is $f(a)+f(b)-f_*$, which in general differs from the exact [Godunov numerical flux](../../../../../godunov-numerical-flux.md). This distinction does not affect the [monotonicity](../../../../../monotonic-function.md) proof.

Here [stability](../../../../../stability-of-a-numerical-method.md) requires the usual [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md). Let the initial values lie in $[m,M]$, and choose

$$
\boxed{r\max_{u\in[m,M]}|f'(u)|\le1.}
$$

A differentiable [convex function](../../../../../convex-function.md) has a continuous [derivative](../../../../../derivative.md) on this interval, so the maximum is finite. Write the three-input update as $H(a,b,c)$. Differentiating gives

$$
H_a=r(f^+)'(a)\ge0,\qquad H_c=-r(f^-)'(c)\ge0,\qquad
H_b=1-r\bigl[(f^+)'(b)-(f^-)'(b)\bigr]=1-r|f'(b)|\ge0.
$$

Thus the update $T$ preserves componentwise order. Constants are fixed, since $H(c,c,c)=c$, so comparison with the constants $m,M$ proves $m\le U_j^n\le M$ for every time level. In particular the same [CFL condition](../../../../../courant-friedrichs-lewy-condition.md) remains applicable. This is a mesh-independent maximum-principle [stability](../../../../../stability-of-a-numerical-method.md) bound.

A stronger [stability](../../../../../stability-of-a-numerical-method.md) statement is contraction in discrete $L^1$. Consider two solutions $U,V$ in the same invariant interval, on a periodic mesh or on the infinite lattice with summable differences. Let $Q=U\vee V$ be their componentwise maximum. [Monotonicity](../../../../../monotonic-function.md) gives $TQ\ge TU,TV$, hence

$$
\sum_j(TU_j-TV_j)^+\le\sum_j(TQ_j-TV_j)
=\sum_j(Q_j-V_j)=\sum_j(U_j-V_j)^+.
$$

The discrete [conservation law](../../../../../conservation-law.md) for the difference gives the equality: on a finite periodic mesh the flux sum cancels exactly, and on the infinite lattice it follows by truncation and the fact that the flux is a [Lipschitz function](../../../../../lipschitz-continuity.md) on $[m,M]$. Interchanging $U,V$ and adding proves

$$
\boxed{h\sum_j|U_j^{n+1}-V_j^{n+1}|\le h\sum_j|U_j^n-V_j^n|.}
$$

This is [L1 contraction of a monotone conservative scheme](../../../../../l1-contraction-of-a-monotone-conservative-scheme.md). Since $T$ commutes with the cell shift, applying this contraction to $U$ and its shift gives $\sum_j|U_{j+1}^{n+1}-U_j^{n+1}|\le\sum_j|U_{j+1}^n-U_j^n|$. The scheme is therefore a [total variation diminishing scheme](../../../../../total-variation-diminishing-scheme.md) as well.

The same order argument proves a [discrete entropy inequality](../../../../../discrete-entropy-inequality.md), explaining why this stable discretization selects [entropy solutions](../../../../../entropy-solution.md) rather than nonphysical expansion [shock waves](../../../../../shock-wave.md). For a constant $c\in[m,M]$, set

$$
Q_c(a,b)=F(a\vee c,b\vee c)-F(a\wedge c,b\wedge c).
$$

Because $T(U\vee c)\ge TU,c$ and $T(U\wedge c)\le TU,c$, their componentwise difference is at least $|TU-c|$. Subtracting their updates gives

$$
|U_j^{n+1}-c|\le|U_j^n-c|-r\bigl[Q_c(U_j^n,U_{j+1}^n)-Q_c(U_{j-1}^n,U_j^n)\bigr].
$$

For constants outside $[m,M]$, the entropy inequality is an equality by the invariant bound and the conservative update. At equal states $Q_c(u,u)=\operatorname{sgn}(u-c)[f(u)-f(c)]$, the [Kruzhkov entropy flux](../../../../../kruzhkov-entropy-flux.md). The flux is a [Lipschitz function](../../../../../lipschitz-continuity.md) on the invariant interval: writing $L=\max|f'|$, the conservative update gives $h\sum_j|U_j^{n+1}-U_j^n|\le2kL\sum_j|U_{j+1}^n-U_j^n|$. This time-translation bound, the invariant bound and the [total variation](../../../../../total-variation.md) estimate give local space-time [compactness](../../../../../compact-space.md) for bounded-variation [initial conditions](../../../../../initial-condition.md) as the mesh is refined; the conservative update passes to the weak [conservation law](../../../../../conservation-law.md), and the displayed inequality passes to its [Kruzhkov entropy inequality](../../../../../kruzhkov-entropy-inequality.md). This identifies the limit as the [entropy solution](../../../../../entropy-solution.md).

Finally the time-step qualification is essential. For the convex [Inviscid Burgers equation](../../../../../inviscid-burgers-equation.md) flux $f(u)=u^2/2$, whose unique [sonic point of a scalar flux](../../../../../sonic-point-of-a-scalar-flux.md) is zero, linearize about a positive constant $U$. The perturbation update becomes $v_j^{n+1}=(1-rU)v_j^n+rUv_{j-1}^n$. At [Fourier frequency](../../../../../fourier-frequency.md) $\pi$ its multiplier is $1-2rU$, with modulus greater than one if $rU>1$. [Wave packets](../../../../../wave-packet.md) near this phase give [linear instability](../../../../../linear-instability.md) even for summable Cauchy perturbations. Thus the assumptions on $f$ imply the [stability](../../../../../stability-of-a-numerical-method.md) results above under the [CFL condition](../../../../../courant-friedrichs-lewy-condition.md), not for arbitrary $k/h$. This is [CFL necessity for explicit Engquist-Osher stability](../../../../../cfl-necessity-for-explicit-engquist-osher-stability.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
