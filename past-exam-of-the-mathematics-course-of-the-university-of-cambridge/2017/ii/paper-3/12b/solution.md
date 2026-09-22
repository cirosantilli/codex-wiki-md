<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

A fraction $1-k$ of adults survives each time step; $k$ is the adult mortality fraction. Adults produce $\mu a_n$ larvae, which mature one step later with recruitment reduced by adult-dependent competition through $1/(1+a_n)$. Eliminating larvae gives the [second-order difference equation](../../../../../second-order-difference-equation.md)

$$
 a_{n+1}=(1-k)a_n+\frac{\mu a_{n-1}}{1+a_n}.
$$

At an [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), either $(a,b)=(0,0)$ or

$$
 \boxed{a_*=\frac\mu k-1,\qquad b_*=\mu\left(\frac\mu k-1\right),\qquad \mu>k.}
$$

Only nonnegative populations are admissible. At extinction the [Jacobian matrix](../../../../../jacobian-matrix.md) is $\begin{pmatrix}1-k&1\\\mu&0\end{pmatrix}$ and its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2-(1-k)\lambda-\mu$. Its positive root exceeds $1$ exactly when $\mu>k$. For $0<\mu<k$ both roots have modulus less than $1$; at $\mu=k$ the roots are $1,-k$, so linearization is marginal. On the nonnegative [state space](../../../../../state-space.md) extinction is still attracting at this equality: if two consecutive adult values are bounded by $M>0$, the next is at most $(1-k)M+kM/(1+a_n)\leq M$, with strict decrease away from zero; the maximum of two consecutive adult values strictly decreases after two steps whenever it is positive; continuity on its bounded state region then excludes a positive limiting maximum. Thus the extinction [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) is unstable exactly when the positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) exists, with equality understood through nonlinear rather than strict linear stability.

At the positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), the trace and [determinant](../../../../../determinant.md) of the [Jacobian matrix](../../../../../jacobian-matrix.md) are $T=1-2k+k^2/\mu$ and $-k$. The [Jury stability criterion](../../../../../jury-stability-criterion.md) for $\lambda^2-T\lambda-k$ requires $1-T-k>0$, $1+T-k>0$ and $1-k>0$. The strict [linear stability analysis](../../../../../linear-stability.md) conditions are

$$
\boxed{\mu>k,\qquad (3k-2)\mu<k^2.}
$$

For $k\leq2/3$ there is no upper bound on $\mu$; for $k>2/3$ the stable region is $k<\mu<k^2/(3k-2)$.

<a id="12b/image-stability-regions-and-equilibrium-branches"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3-stability.png)

**[Figure 1](#12b/image-stability-regions-and-equilibrium-branches). Stability regions and equilibrium branches**.

At the lower boundary $\mu=k$, the positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) merges with extinction, with a multiplier $+1$ and slow recovery. At the upper boundary a multiplier reaches $-1$ (the other is $k$), giving alternating adult/larval fluctuations. The nonlinear map confirms a supercritical [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md), as follows. For $k>2/3$, put $h=1-k$ and $\mu_c=k^2/(3k-2)$. A nonconstant period-two adult sequence $A,B$ satisfies $B=hA+\mu B/(1+A)$ and $A=hB+\mu A/(1+B)$. Subtracting and adding these equations gives

$$
 S=A+B=\frac{\mu-1-h}{h},\qquad P=AB=\frac{hS(S+1)}{1+h},\qquad
 (A-B)^2=\frac{S[(1-3h)S-4h]}{1+h}.
$$

Thus positive unequal values emerge for $\mu>\mu_c$, with amplitude proportional to $\sqrt{\mu-\mu_c}$. The two larval phases are $\mu B,\mu A$. If $T_2,\Delta_2$ are the trace and determinant of the two-step [Jacobian matrix](../../../../../jacobian-matrix.md), direct multiplication gives

$$
 \Delta_2=\frac{(1+h)\mu}{S+1},\qquad
 1-T_2+\Delta_2=\frac{Sh(1+h)[(1-3h)S-4h]}{(S+1)\mu}>0.
$$

At onset $\Delta_2=k^2<1$ and $T_2=1+k^2$, so the other two strict [Jury stability criterion](../../../../../jury-stability-criterion.md) inequalities hold for sufficiently small positive $\mu-\mu_c$. Hence **just beyond the upper boundary, a stable period-two population cycle replaces the stable equilibrium**. This is a local conclusion, not stability for arbitrarily large reproduction rates.

At the upper boundary itself, the positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) is still locally asymptotically stable, despite its multiplier $-1$. To decide this equality case, apply the [centre manifold theorem for a discrete dynamical system](../../../../../centre-manifold-theorem-for-a-discrete-dynamical-system.md). Put $u=a-a_*$ and write the centre graph as $b-b_*=H(u)$ with $H'(0)=-\mu_c$. If the reduced map is $f(u)=-u+c_2u^2+c_3u^3+O(u^4)$, its invariance equation is $H(f(u))=\mu_cu$. Expanding the original recruitment map and this equation through cubic order gives

$$
c_2=\frac{(2-k)(3k-2)}{k(1-k)},\qquad
c_3+c_2^2=\frac{(2-k)(3k-2)^2}{k^2(k+1)}>0.
$$

Consequently $f^2(u)=u-2(c_3+c_2^2)u^3+O(u^4)$. The [stability at a nondegenerate flip bifurcation](../../../../../stability-at-a-nondegenerate-flip-bifurcation.md) criterion shows algebraic attraction on the centre direction; the transverse multiplier $k$ has [modulus](../../../../../modulus.md) less than one. Including this boundary, the complete local asymptotic-stability condition for a positive population is therefore

$$
\boxed{\mu>k,\qquad (3k-2)\mu\leq k^2.}
$$

The shaded figure shows the strict linear-stability region; its upper boundary adds this nonhyperbolic attracting case.

[Demographic stochasticity](../../../../../demographic-stochasticity.md) near the lower boundary can lead to absorption at extinction; near the upper boundary it excites alternating fluctuations and can blur the deterministic [period-doubling bifurcation](../../../../../period-doubling-bifurcation.md). These qualitative predictions depend on the chosen stochastic recruitment and mortality rules.

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
