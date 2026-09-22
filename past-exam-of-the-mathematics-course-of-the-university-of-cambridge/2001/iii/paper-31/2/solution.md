<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the sign convention

$$
L_b(x,\lambda)=f(x)-\lambda^T(h(x)-b),\qquad x\in X,\quad\lambda\in\mathbb R^m.
$$

This is the [optimization Lagrangian](../../../../../optimization-lagrangian.md); equality-constraint [Lagrange multipliers](../../../../../lagrange-multiplier.md) are unrestricted in sign. The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) for minimization says: if $x_*\in X$ satisfies $h(x_*)=b$ and globally minimizes $L_b(\,\cdot\,,\lambda_*)$ on $X$ for some $\lambda_*$, then it globally minimizes the constrained [objective function](../../../../../objective-function.md). Indeed, for every feasible $x$,

$$
f(x)=L_b(x,\lambda_*)\ge L_b(x_*,\lambda_*)=f(x_*).
$$

This is a full global certificate, not merely stationarity. No convexity is needed for the implication, although convexity commonly supplies the required global [optimization Lagrangian](../../../../../optimization-lagrangian.md) minimum.

Let $\phi(u)=\inf\{f(x):x\in X,\ h(x)=u\}$, setting $\inf\varnothing=+\infty$, and assume $\phi(b)$ is finite. The [Strong Lagrangian property](../../../../../strong-lagrangian-property.md) at $b$ means that a finite multiplier attains the constrained value as an unconstrained lower bound:

$$
\boxed{\inf_{x\in X}L_b(x,\lambda_*)=\phi(b).}
$$

This includes dual attainment, but need not include primal attainment. A [non-vertical supporting hyperplane of a value function](../../../../../non-vertical-supporting-hyperplane-of-a-value-function.md) at $b$ has a finite slope $\lambda_*$ and supports the [epigraph](../../../../../epigraph.md) from below:

$$
\phi(u)\ge\phi(b)+\lambda_*^T(u-b)\quad\text{for every }u.
$$

If this inequality holds, then for every $x\in X$,

$$
f(x)\ge\phi(h(x))\ge\phi(b)+\lambda_*^T(h(x)-b),
$$

so $\inf_XL_b(x,\lambda_*)\ge\phi(b)$. Conversely restricting the infimum to $h(x)=b$ gives $\inf_XL_b\le\phi(b)$, even if the primal infimum is approached only by a sequence. Thus equality holds. In the reverse direction, the Strong [optimization Lagrangian](../../../../../optimization-lagrangian.md) identity implies $f(x)-\lambda_*^T(h(x)-b)\ge\phi(b)$ for every $x$. Taking the infimum over $h(x)=u$ yields the supporting inequality, with empty fibres causing no problem. This proves both implications without a convexity or attainment assumption beyond finite $\phi(b)$.

For the advertising calculation, measure the budget in thousands of pounds by $B=a/1000$. Requiring the full budget to be spent gives $3x+y=B$, with $x,y\ge0$. Substitute $y=B-3x$ to reduce the [maximization problem](../../../../../maximization-problem.md) to

$$
F_B(x)=-14x^2+(7B-1)x+3B-B^2,\qquad 0\le x\le B/3.
$$

Its [second derivative](../../../../../second-derivative.md) is $-28$, so the unique constrained maximum is obtained by clipping the [stationary point](../../../../../stationary-point.md):

$$
\boxed{(x_*,y_*)=
\begin{cases}
(0,B),&0\le B\le1/7,\\
(B/4-1/28,\ B/4+3/28),&B\ge1/7.
\end{cases}}
$$

The upper constraint never clips the interior formula because $B/4-1/28<B/3$ for $B\ge0$. The maximal revenue in thousands of pounds is

$$
R(B)=
\begin{cases}
3B-B^2,&0\le B\le1/7,\\
-B^2/8+11B/4+1/56,&B\ge1/7.
\end{cases}
$$

Equivalently the revenue [Hessian](../../../../../hessian-matrix.md) is $\begin{pmatrix}-4&1\\1&-2\end{pmatrix}$, [negative definite](../../../../../negative-definite-matrix.md) since its leading minor is negative and its [determinant](../../../../../determinant.md) is seven. Thus the full-budget affine feasible set has a unique global maximum.

At the two requested budgets,

$$
\begin{array}{c|c|c|c}
a&x_*&y_*&R(a/1000)\\ \hline
1000&3/14&5/14&37/14\\
10000&69/28&73/28&841/56
\end{array}
$$

The units in the middle columns are minutes; the last column is thousands of pounds. Revenue measured in pounds is $G(a)=1000R(a/1000)$, so

$$
\boxed{G'(1000)=\frac52,\qquad G'(10000)=\frac14.}
$$

An additional advertising pound therefore increases optimized revenue locally by £2.50 at the smaller budget and £0.25 at the larger budget. These are marginal rates, not exact finite-difference increments: on the interior branch $G(a+1)-G(a)=G'(a)-1/8000$.

The maximization multiplier in $f(x,y)-\mu(3x+y-B)$ equals $R'(B)=(11-B)/4$ on the interior branch. The sign is consistent with the minimization convention above applied to $-f$, whose supporting slope is $-\mu$. If spending is only capped by the budget, rather than required to equal it, these same answers apply at the two budgets. Beyond £11,000 the unconstrained maximum $(x,y)=(19/7,20/7)$ is affordable, so further allowed spending is unused and the capped-budget value is constant; forced full spending would instead lower revenue.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
