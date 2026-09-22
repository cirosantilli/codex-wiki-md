<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $a,b,e$ be fractions of patches occupied by the two competitors and empty, with $a+b+e=1$. Assume well-mixed propagule dispersal, equal independent fire extinction rate $m>0$, colonization constants $c_A>c_B>0$, and net replacement advantage $q=k_B-k_A>0$ for the poorer colonizer. The [Levins metapopulation model](../../../../../levins-metapopulation-model.md) with replacement is

$$
\dot a=a(c_Ae-m-qb),\qquad
\dot b=b(c_Be-m+qa),\qquad
\dot e=m(a+b)-e(c_Aa+c_Bb).
$$

Replacement fluxes $k_Bab$ and $k_Aab$ cancel in the total occupancy equation. At every face the outward flux is zero or points into the patch [probability simplex](../../../../../probability-simplex.md), so these equations preserve valid fractions. The constants include both propagule arrival and establishment [probability](../../../../../probability.md); the model does not require unequal fire susceptibility.

Put $\Delta c=c_A-c_B$. Solving the two occupied-patch balances and their sum constraint gives

$$
\boxed{e_* =\frac q{q+\Delta c},\qquad
 a_* =\frac mq-\frac{c_B}{q+\Delta c},\qquad
 b_* =\frac{c_A}{q+\Delta c}-\frac mq.}
$$

Thus strict coexistence is equivalent to

$$
\boxed{\frac{qc_B}{q+\Delta c}<m<\frac{qc_A}{q+\Delta c}.}
$$

Too little disturbance lets the better competitor exclude the colonizer; too much disturbance favors colonization or destroys occupancy. A positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) automatically has $m<c_A$. If the poorer colonizer cannot survive alone, coexistence can nevertheless be possible because it repeatedly replaces established patches of the better colonizer.

These bounds also have an invasion interpretation. The $A$-only [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is $a=1-m/c_A$ when $c_A>m$; the growth rate of rare $B$ there is $q-m(q+\Delta c)/c_A$, positive at the upper-bound condition above. At a feasible $B$-only [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) the rare-$A$ growth is $-q+m(q+\Delta c)/c_B$, giving the lower bound. At coexistence the occupied-patch [Jacobian matrix](../../../../../jacobian-matrix.md) has [trace](../../../../../matrix-trace.md) $-c_Aa_*-c_Bb_*<0$ and [determinant](../../../../../determinant.md) $a_*b_*q(q+\Delta c)>0$, proving local asymptotic stability. The [Bendixson-Dulac criterion](../../../../../bendixson-dulac-theorem.md) with multiplier $1/(ab)$ gives divergence $-c_A/b-c_B/a<0$ in the interior, excluding periodic competition cycles.

To specify selection, a monotone tradeoff alone is insufficient: one must say how two different trait values determine replacement. A natural model uses a trait $x$ with increasing competitive ability $B(x)$ and decreasing colonization $c(x)$, and net replacement $B(y)-B(x)$ by a mutant $y$ against a resident $x$. The resident [metapopulation](../../../../../metapopulation.md) occupies $1-m/c(x)$, requiring $c(x)>m$. The rare-mutant per-capita growth, or invasion fitness, is

$$
f(y,x)=m\left[\frac{c(y)}{c(x)}-1\right]+[B(y)-B(x)]\left[1-\frac m{c(x)}\right].
$$

It is zero at $y=x$. Differentiating with respect to the mutant trait gives the selective pressure

$$
\boxed{g(x)=\partial_yf(x,x)=\frac{mc'(x)}{c(x)}+\left[1-\frac m{c(x)}\right]B'(x).}
$$

Higher colonization is valuable in empty habitat; higher competitive ability is valuable where the resident already occupies patches. This is [colonization-competition tradeoff invasion fitness](../../../../../colonization-competition-tradeoff-invasion-fitness.md).

At an interior candidate for a local [evolutionarily stable strategy](../../../../../evolutionarily-stable-strategy.md), $g(x_*)=0$. A strict, nondegenerate local [evolutionarily stable strategy](../../../../../evolutionarily-stable-strategy.md) follows if

$$
\partial_{yy}f(x_*,x_*)=\frac{mc''(x_*)}{c(x_*)}+\left[1-\frac m{c(x_*)}\right]B''(x_*)<0,
$$

since nearby distinct mutants then have negative invasion fitness. For a strict global [evolutionarily stable strategy](../../../../../evolutionarily-stable-strategy.md), every feasible distinct mutant must satisfy

$$
\boxed{mc(y)+[c(x_*)-m]B(y)<mc(x_*)+[c(x_*)-m]B(x_*)\quad(y\ne x_*).}
$$

This is the supporting-line condition on the tradeoff curve. At a trait boundary replace the vanishing-gradient condition by the appropriate one-sided inequality. Equality against another mutant, or zero local curvature, needs the second condition of evolutionary stability or higher-order terms; the strict tests above are sufficient and are the usual nondegenerate conditions, not a claim that every tie is unstable.

For evolutionary approach to a singular point, the [selection gradient](../../../../../selection-gradient.md) must also point toward it, locally $g'(x_*)<0$. This is logically distinct from testing mutant fitness. In this particular additive-ability model with $c'<0<B'$, negative mutant curvature implies negative $g'$ because

$$
g'(x)=\partial_{yy}f(x,x)+\frac{mc'(x)[B'(x)-c'(x)]}{c(x)^2}.
$$

If replacement instead has a general kernel $\kappa(y,x)$, replace $B(y)-B(x)$ in $f$ by that kernel and differentiate it; monotonicity does not justify importing the displayed additive formula without that modeling assumption. **The tradeoff shape, disturbance rate and replacement law together determine selection and local or global uninvadability.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
