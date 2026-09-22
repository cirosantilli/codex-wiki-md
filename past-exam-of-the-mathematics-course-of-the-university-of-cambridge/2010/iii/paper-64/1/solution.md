<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A sufficient set of assumptions is that $L$ is a densely defined [closed operator](../../../../../closed-linear-operator.md) on the [Hilbert space](../../../../../hilbert-space-split.md) $H$, generating an [analytic semigroup](../../../../../analytic-semigroup.md) $S(t)$, and that $f\in C^{0,\theta}([0,T],H)$ for some $0<\theta\leq1$. For an operator criterion, one may assume that $A=\omega I-L$ is a [sectorial operator](../../../../../sectorial-operator.md) of angle less than $\pi/2$, with dense domain. The [analytic semigroup](../../../../../analytic-semigroup.md) then satisfies, on a fixed finite time interval,

$$
\|S(t)\|\leq M_T,\qquad \|LS(t)\|\leq C_T/t,\qquad S(t)H\subset D(L)\quad(t>0).
$$

The [Hölder continuity](../../../../../holder-condition.md) assumption means $\|f(t)-f(s)\|_H\leq K|t-s|^\theta$. It supplies time regularity of the forcing, not spatial membership of $f(t)$ in $D(L)$.

With initial datum $u_0\in H$, a [classical solution of an abstract Cauchy problem](../../../../../classical-solution-of-an-abstract-cauchy-problem.md) means

$$
u\in C([0,T],H)\cap C^1((0,T],H),\qquad u(t)\in D(L),\qquad Lu\in C((0,T],H),
$$

with the evolution identity holding in $H$ at positive times and $u(t)\to u_0$ in $H$. Equivalently, the positive-time domain continuity is in the [graph norm](../../../../../graph-norm.md). If the definition requires differentiability also at zero, assume additionally $u_0\in D(L)$; the proof below then gives $u\in C^1([0,T],H)\cap C([0,T],D(L))$.

The [variation-of-constants formula](../../../../../variation-of-constants-formula.md) gives the candidate

$$
\boxed{u(t)=S(t)u_0+\int_0^tS(t-s)f(s)\,ds.}
$$

The integral is a [Bochner integral](../../../../../bochner-integral.md). Boundedness of $S$ and continuity of $f$ make the expression continuous into $H$, and its integral term tends to zero with $t$. Thus it is a [mild solution of an abstract Cauchy problem](../../../../../mild-solution-of-an-abstract-cauchy-problem.md) with the correct initial value. The issue is showing that its integral term lies in the domain of the unbounded [linear operator](../../../../../linear-operator.md) $L$.

Write $v(t)=\int_0^tS(r)f(t-r)\,dr$. For $\varepsilon>0$, the truncated integral $v_\varepsilon(t)=\int_\varepsilon^tS(r)f(t-r)\,dr$ lies in $D(L)$. Subtract the current forcing before applying $L$:

$$
Lv_\varepsilon(t)=\int_\varepsilon^tLS(r)[f(t-r)-f(t)]\,dr+[S(t)-S(\varepsilon)]f(t).
$$

Here the last term follows by integrating $LS(r)f(t)=\frac d{dr}S(r)f(t)$ away from zero; it does not assume that $f(t)\in D(L)$. The first integrand satisfies

$$
\|LS(r)[f(t-r)-f(t)]\|_H\leq C_TK r^{\theta-1},\qquad
\int_0^t r^{\theta-1}\,dr=t^\theta/\theta<\infty.
$$

Since $v_\varepsilon(t)\to v(t)$ in $H$ and the displayed images also converge, the [closed operator](../../../../../closed-linear-operator.md) property gives

$$
v(t)\in D(L),\qquad Lv(t)=\int_0^tLS(r)[f(t-r)-f(t)]\,dr+[S(t)-I]f(t).
$$

This is the reason for the [Hölder continuity](../../../../../holder-condition.md) assumption: the unsplit estimate would have the nonintegrable factor $r^{-1}$. Merely knowing that $f$ is continuous does not provide the integrable bound needed here. More generally, a modulus of continuity $\eta$ satisfying $\int_0^1\eta(r)\,dr/r<\infty$ suffices for this argument; a positive [Hölder exponent](../../../../../holder-exponent.md) is a convenient sufficient hypothesis.

The formula also proves continuity of $Lv$ at positive times. On compact positive-time intervals, split the integral at a small $r=\varepsilon$: its short part is uniformly bounded by $C\varepsilon^\theta$, while the remaining part is continuous by the [strongly continuous semigroup](../../../../../c0-semigroup.md) property and ordinary dominated convergence. Together with analytic smoothing of $S(t)u_0$, this makes $Lu$ continuous at positive times. The [semigroup property](../../../../../semigroup-property.md) gives

$$
u(t+h)=S(h)u(t)+\int_0^hS(h-r)f(t+r)\,dr.
$$

Because $u(t)\in D(L)$, division of this identity by $h$ after subtracting $u(t)$ gives the continuous right derivative $Lu(t)+f(t)$. The left derivative agrees by the same identity and continuity of $Lu+f$. Thus $u'=Lu+f$, proving existence of the [classical solution of an abstract Cauchy problem](../../../../../classical-solution-of-an-abstract-cauchy-problem.md) on the entire given finite interval, and in particular local existence.

For uniqueness, the difference $h$ of two such [classical solutions of an abstract Cauchy problem](../../../../../classical-solution-of-an-abstract-cauchy-problem.md) satisfies $h'=Lh$ and $h(0)=0$. For $0<\varepsilon<t$, differentiation of $S(t-s)h(s)$ on $[\varepsilon,t]$ gives zero, so $h(t)=S(t-\varepsilon)h(\varepsilon)$. Letting $\varepsilon\downarrow0$ yields $h(t)=0$. Finally, if $u_0\in D(L)$, then $LS(t)u_0=S(t)Lu_0\to Lu_0$, and the expression for $Lv(t)$ tends to zero. Hence $u'(t)\to Lu_0+f(0)$ and the stronger time-zero regularity follows. **The solution is unique; the forcing regularity controls the singularity in the differentiated integral.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
