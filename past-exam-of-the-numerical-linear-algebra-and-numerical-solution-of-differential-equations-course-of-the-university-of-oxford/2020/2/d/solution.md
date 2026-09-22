<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The coefficients of this [linear multistep method](../../../../linear-multistep-method-split.md) are $\alpha_0=b$, $\alpha_1=-a$, $\alpha_2=1$ and $\beta_0=\beta_1=0$, $\beta_2=c$. Substitution into the [order of a numerical method](../../../../order-of-a-numerical-method.md) conditions gives

$$
1-a+b=0,\qquad 2-a-c=0,\qquad 2-\frac a2-2c=0.
$$

The second equation gives $c=2-a$; substituting this into the third gives $-2+3a/2=0$. Consequently there is exactly one second-order choice,

$$
\boxed{a=\frac43,\qquad b=\frac13,\qquad c=\frac23.}
$$

The resulting scheme is the [BDF2 method](../../../../second-order-backward-differentiation-formula.md),

$$
3Y_{n+2}-4Y_{n+1}+Y_n=2h f(x_{n+2},Y_{n+2}).
$$

For a $C^4$ exact solution, [Taylor's theorem](../../../../taylor-s-theorem.md) in the original normalization gives the exact leading order defect

$$
\begin{aligned}
T_n(h)
&=\frac{y(x_n+2h)-\frac43y(x_n+h)+\frac13y(x_n)}h-\frac23y'(x_n+2h)\\
&=-\frac29h^2y'''(x_n)+O(h^3).
\end{aligned}
$$

In particular the coefficient $-2/9$ is nonzero: the method has formal order exactly two, rather than three. Bounded third derivatives already suffice for the uniform estimate $T_n(h)=O(h^2)$; the stronger smoothness above only makes the displayed remainder immediate. Multiplying the recurrence by $3/2$ instead gives the common derivative normalization with leading defect $-h^2y'''(x_n)/3$.

The first of the [characteristic polynomials of a linear multistep method](../../../../characteristic-polynomials-of-a-linear-multistep-method.md) is

$$
\rho(z)=z^2-\frac43z+\frac13=(z-1)\left(z-\frac13\right).
$$

Both roots are simple and lie in the closed unit disk, so the [root condition for a multistep method](../../../../root-condition-for-a-multistep-method.md) proves [zero-stability](../../../../zero-stability.md).

The [Dahlquist equivalence theorem](../../../../dahlquist-equivalence-theorem.md) states that, for fixed-coefficient [linear multistep methods](../../../../linear-multistep-method-split.md) on the usual class of [initial value problems](../../../../initial-value-problem.md) with a right-hand side continuous in $x$ and uniformly [Lipschitz continuous](../../../../lipschitz-continuity.md) in $y$, [convergence of a numerical method](../../../../convergence-of-a-numerical-method.md) for every such problem and every convergent set of starting values is equivalent to [consistency of a numerical method](../../../../consistency-of-a-numerical-method.md) and [zero-stability](../../../../zero-stability.md). The statement is on fixed finite intervals where the exact solution exists, with implicit updates well defined. Its order estimate says that a [zero-stable](../../../../zero-stability.md) method with $T_n(h)=O(h^p)$ and starting errors $O(h^p)$ has [global error](../../../../global-discretization-error.md) $O(h^p)$ under the corresponding solution smoothness and [Lipschitz continuity](../../../../lipschitz-continuity.md) assumptions; merely convergent starting values do not ensure the order-$p$ rate.

For this application, sufficient assumptions are a unique solution $y\in C^3([x_0,x_0+T])$, a uniform [Lipschitz continuity](../../../../lipschitz-continuity.md) bound $L$ in $y$ on a neighborhood of its graph, and the nearby solution branch of each implicit update. For sufficiently small $h$, the map

$$
z\longmapsto\frac43Y_{n+1}-\frac13Y_n+\frac23h f(x_{n+2},z)
$$

is a [contraction mapping](../../../../contraction-mapping.md) with factor at most $2hL/3<1$ on a suitable small closed neighborhood. The [Banach fixed-point theorem](../../../../contraction-mapping-theorem.md) supplies local solvability of the nearby update. With starting errors

$$
|Y_0-y(x_0)|+|Y_1-y(x_0+h)|=O(h^2),
$$

the order estimate gives

$$
\max_{0\leq nh\leq T}|Y_n-y(x_n)|\leq C_T\left(|Y_0-y(x_0)|+|Y_1-y(x_0+h)|+\max_n|T_n(h)|\right)=O(h^2).
$$

Thus the [BDF2 method](../../../../second-order-backward-differentiation-formula.md) is second-order convergent under these standard hypotheses. Exact $Y_0=y(x_0)$ together with one [Euler method](../../../../euler-method.md) step for $Y_1$ already gives the required starting error when $y''$ is bounded, since only one starting step is taken.

The question's assumption of [continuity](../../../../continuous-function.md) of $f$ alone does not establish uniqueness, the needed solution smoothness, or this uniform convergence estimate. The added [Lipschitz continuity](../../../../lipschitz-continuity.md) condition is a sufficient hypothesis for the theorem used here; its failure does not imply that every particular [initial value problem](../../../../initial-value-problem.md) is nonunique or that its numerical approximations cannot converge.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
