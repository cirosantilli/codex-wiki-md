<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [fixed singularity of a complex differential equation](../../../../../fixed-singularity-of-a-complex-differential-equation.md) has a location determined by the coefficients, independently of the initial value. A [movable singularity of a complex differential equation](../../../../../movable-singularity-of-a-complex-differential-equation.md) belongs to an individual continued solution and changes location when the initial value changes. For example, $w'=w^2$ has the movable [pole](../../../../../pole.md) $z=c$ in $w=-1/(z-c)$. A fixed exceptional location need not be singular for every solution.

The precise first-order form of the [Painlevé determinateness theorem](../../../../../painleve-determinateness-theorem.md) needed here is as follows. Let $w'=A(z,w)$ be rational in $w$, with coefficients [meromorphic](../../../../../meromorphic-function.md) in $z$ on the chosen independent-variable surface. Algebraic coefficients can be made single valued on their own surface. Exclude the fixed coefficient singularities and exceptional fibres where a reduced numerator and denominator vanish together, working also in the dependent coordinate $v=1/w$. If a solution is continued along an arc $\gamma:[0,1)\to U$ with endpoint $z_*=\lim_{t\to1}\gamma(t)$ outside that exceptional set, then **$w(\gamma(t))$ has a definite finite or infinite limit**. Any singularity there is a [pole](../../../../../pole.md) or an [algebraic branch point](../../../../../algebraic-branch-point.md); there is no movable essential or logarithmic singularity. The standard rectifiable-arc formulation is included in this statement.

Here is a proof. First suppose a sequence along the arc has $(z_n,w_n)\to(z_*,w_*)$ at a point where the vector field is [holomorphic](../../../../../complex-differentiability-at-a-point.md). Choose a smaller closed bidisc about this point. Uniform bounds on the vector field and its dependent-variable [derivative](../../../../../derivative.md) give, by the integral [contraction mapping](../../../../../contraction-mapping.md) proof, one radius $r>0$ on which every solution starting sufficiently close to $(z_*,w_*)$ exists and remains bounded. For large $n$, the solution through $(z_n,w_n)$ is therefore defined on a fixed disc about $z_*$. The entire sufficiently late tail of $\gamma$ lies in that disc. Uniqueness identifies the original continued solution with this local solution throughout that tail, so the solution extends through $z_*$ and has a limit. The same argument applies to an ordinary point in the reciprocal coordinate $v=1/w$.

If the limit did not exist, consider the cluster set $K$ in the dependent-variable [Riemann sphere](../../../../../riemann-sphere.md):

$$
K=\bigcap_{s<1}\overline{\{w(\gamma(t)):s\le t<1\}}.
$$

Each closed tail is compact and connected, and these sets are nested; hence $K$ is nonempty, compact and connected. The preceding paragraph excludes every ordinary point from $K$. At $z_*$ the rational vector field has only finitely many nonordinary dependent values, in both coordinate charts: an entire fibre of singular points was excluded among the fixed exceptions. Thus $K$ is a connected subset of a finite set, so it is a singleton. Compactness then forces convergence to its unique point, contradicting the assumed lack of a limit. This proves determinateness.

It remains to determine the local type rather than merely the limit. At a finite limiting value $w_*$ which is a pole of the vector field, write the reduced equation as $w'=P/Q$. Since $z_*$ is not exceptional, $P(z_*,w_*)\ne0$, and the inverse equation

$$
\frac{dz}{dw}=\frac{Q(z,w)}{P(z,w)}
$$

is [holomorphic](../../../../../complex-differentiability-at-a-point.md) near $(z_*,w_*)$. The [holomorphic dependence of ordinary differential equations on parameters](../../../../../holomorphic-dependence-of-ordinary-differential-equations-on-parameters.md) makes its local solution curves jointly [holomorphic](../../../../../complex-differentiability-at-a-point.md) in $w$ and their initial $z$ values. In particular, the value at the transverse line $w=w_*$ is a [holomorphic](../../../../../complex-differentiability-at-a-point.md) first integral labelling these curves. The original graph has constant label; taking its endpoint limit shows that it lies on the inverse solution through $(z_*,w_*)$. That inverse solution cannot be the vertical curve $z\equiv z_*$: this would require $Q(z_*,w)$ to vanish identically near $w_*$, an excluded fixed singular fibre. Consequently its [power series](../../../../../power-series.md) has a first nonzero term,

$$
z(w)-z_*=c(w-w_*)^k+O((w-w_*)^{k+1}),\qquad c\ne0.
$$

Here $k\ge2$ at a vector-field pole. Factor the right side as $(w-w_*)^k$ times a nonvanishing [holomorphic function](../../../../../holomorphic-function.md) and take its local $k$th root. This gives a new dependent coordinate with nonzero [derivative](../../../../../derivative.md), and the [holomorphic inverse function theorem](../../../../../holomorphic-inverse-function-theorem.md) expresses $w$ as a convergent [power series](../../../../../power-series.md) in $(z-z_*)^{1/k}$. Thus the singularity is an [algebraic branch point](../../../../../algebraic-branch-point.md). At an infinite limit, repeat the argument for $v=1/w$. An ordinary zero of $v$ gives a [pole](../../../../../pole.md) of $w$, while a finite ramification of $v$ gives an algebraic pole branch. This proves the asserted local types and the theorem.

For the given equation, the finite-coordinate rational field is

$$
A(z,w)=\frac{w}{(z+1)(w^2-z^2)}.
$$

The whole fibre $z=-1$ is singular in the displayed coefficient, and at $(z,w)=(0,0)$ the reduced numerator and denominator vanish together. Hence the finite fixed exceptional set is $\{-1,0\}$. Away from these two locations, the only possible finite dependent limits at a singularity are $w_* =\sigma z_*$, with $\sigma=\pm1$.

At such a point the inverse equation is

$$
z_w=\frac{(z+1)(w^2-z^2)}w.
$$

It is [holomorphic](../../../../../complex-differentiability-at-a-point.md) when $z_*\ne0,-1$ and $w_* =\sigma z_*$. Its inverse solution satisfies $z_w(w_*)=0$, and differentiation gives

$$
z_{ww}(w_*)=(z_*+1)\left(1+\frac{z_*^2}{w_*^2}\right)=2(z_*+1).
$$

Therefore

$$
z-z_*=(z_*+1)(w-w_*)^2+O((w-w_*)^3),
$$

and

$$
\boxed{w(z)=\sigma z_*\;\pm\sqrt{\frac{z-z_*}{z_*+1}}+O(z-z_*).}
$$

These are genuine square-root [algebraic branch points](../../../../../algebraic-branch-point.md). The inverse solutions can be based at arbitrary $z_*\notin\{0,-1\}$ and then continued to nearby ordinary initial points. Their distinct branch locations require different initial data, so **these branch points are movable**. The signs specify the two inverse branches near each of the two values $w_* =\pm z_*$.

There are **no movable poles**. Indeed the reciprocal equation is

$$
v'=-\frac{v^3}{(z+1)(1-z^2v^2)}.
$$

For every finite $z\ne-1$ it is [holomorphic](../../../../../complex-differentiability-at-a-point.md) at $v=0$, and $v\equiv0$ is its unique solution with zero initial value. A nonzero reciprocal solution therefore cannot reach zero there. This rules out both an ordinary pole and an infinite algebraic branch at a movable finite location. Together with the theorem, it exhausts the finite movable singularities.

The fixed point zero must not be mistaken for a generic movable collision. It is ordinary for solutions with $w(0)\ne0$. But solutions reaching $w=0$ can have a fixed square-root singularity. To construct them rather than just balance powers, set $z(w)=w^2h(w)$ in the inverse equation. The equation for $h$ is

$$
wh'=1-2h+w^2(h-h^2)-w^4h^3,\qquad h(0)=\tfrac12.
$$

Equivalently,

$$
h(w)=\int_0^1t\left[1+w^2t^2\{h(wt)-h(wt)^2\}-w^4t^4h(wt)^3\right]dt.
$$

On a small disc this is a [contraction mapping](../../../../../contraction-mapping.md) of the closed ball $\|h-1/2\|_\infty\le1/4$: both its departure from $1/2$ and its Lipschitz constant are $O(r^2)$. Its unique [holomorphic](../../../../../complex-differentiability-at-a-point.md) fixed point gives $z=w^2/2+O(w^4)$. Thus

$$
w(z)=\pm\sqrt{2z}\,(1+O(z))
$$

is a genuine branch at the fixed location zero. The zero solution itself extends through zero as a function, although the original displayed coefficient is undefined at $(0,0)$.

The point $-1$ can produce a fixed nonalgebraic singularity. For an explicit example take $z=-1+x$ real, $0<x<x_0<1$, and $w=iy$ with initial $y>2$. Put $q=y^2$ and $L=-\log x$. Then

$$
\frac{dq}{dL}=\frac{2q}{q+(x-1)^2}.
$$

As $L$ increases, $q$ increases, its derivative is bounded above by $2$ and bounded below by a positive constant, and therefore the solution exists for all large $L$ and $q\to\infty$. The derivative then tends to $2$, so $q/L\to2$. Consequently

$$
w(z)^2\sim2\log(z+1)\qquad(z\downarrow-1).
$$

This is unbounded but grows more slowly than every negative power of $z+1$. It cannot be a meromorphic pole even after a finite ramified substitution, demonstrating an actual fixed singularity with logarithmic growth. The determinateness theorem does not exclude such behavior at fixed exceptions.

Finally, on the independent-variable [Riemann sphere](../../../../../riemann-sphere.md) use $t=1/z$. For finite $w$ the transformed equation is

$$
\frac{dw}{dt}=\frac{tw}{(1+t)(1-t^2w^2)},
$$

which is ordinary at $t=0$. At simultaneous $z=\infty$, $w=\infty$, however, the reciprocal field is

$$
\frac{dv}{dt}=-\frac{tv^3}{(1+t)(v^2-t^2)},
$$

with an indeterminate point at $(t,v)=(0,0)$. Thus infinity is an additional fixed exceptional location on the sphere, rather than an unavoidable singularity of solutions with finite limiting value. There are solutions escaping to infinity there: for real initial data $w(z_0)>z_0>0$, the difference $d=w-z$ stays positive, since its derivative becomes positive as $d\downarrow0$. Moreover $d'\le0$ when $d\ge1$, so $0<d\le\max(1,d(z_0))$. Such a solution continues for all positive $z$, with $w=z+O(1)\to\infty$.

**In the finite plane, the fixed exceptional locations are $0,-1$; all other solution singularities are movable square-root branches at $w=\pm z$, and there are no movable poles. On the sphere, infinity is also a fixed exception at the infinite dependent value.** Being fixed or movable describes the base location, not merely whether the coefficient contains the factors $w-z$ and $w+z$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
