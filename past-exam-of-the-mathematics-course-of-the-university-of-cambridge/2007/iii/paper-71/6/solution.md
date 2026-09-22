<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [collocation Runge-Kutta method](../../../../../collocation-runge-kutta-method.md) approximates an [ordinary differential equation](../../../../../ordinary-differential-equation.md) by a polynomial whose derivative agrees with the vector field at selected times. Let $s$ distinct nodes be $c_i\in[0,1]$, and consider the possibly nonautonomous equation $y'=f(t,y)$. On a step from $(t_n,y_n)$, choose a polynomial $U(\tau)$ of degree at most $s$, with $U(0)=y_n$, such that $U'(c_i)=h f(t_n+c_i h,U(c_i))$. Here $\tau=(t-t_n)/h$ is scaled time; the numerical endpoint is $y_{n+1}=U(1)$.

Let $\ell_j$ be the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) equal to one at $c_j$ and zero at the other nodes, and set $k_j=f(t_n+c_jh,U(c_j))$. Interpolation of the polynomial derivative gives

$$
U'(\tau)=h\sum_{j=1}^s\ell_j(\tau)k_j,\qquad U(\tau)=y_n+h\sum_{j=1}^s\left(\int_0^\tau\ell_j(v)dv\right)k_j.
$$

Evaluating at the nodes and endpoint derives the [Runge-Kutta method](../../../../../runge-kutta-method.md) coefficients:

$$
\boxed{a_{ij}=\int_0^{c_i}\ell_j(v)dv,\qquad b_j=\int_0^1\ell_j(v)dv,\qquad k_i=f\left(t_n+c_ih,y_n+h\sum_j a_{ij}k_j\right).}
$$

Thus collocation is a specific family of generally implicit [RK methods](../../../../../runge-kutta-method.md), not a separate update mechanism. The identity $\sum_j\ell_j=1$ gives $A\mathbf1=c$ and $\sum_jb_j=1$, the [collocation tableau row-sum identity](../../../../../collocation-tableau-row-sum-identity.md). For sufficiently small $h$, a vector field with Lipschitz constant $L$ gives a contraction of the stage map when $hL\max_i\sum_j|a_{ij}|<1$, on a suitable bounded neighborhood. The [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) then gives a unique nearby stage solution. Equivalently smooth stage equations have identity derivative in the stage variables at $h=0$, so the [inverse function theorem](../../../../../inverse-function-theorem.md) gives a smooth nearby branch. Arbitrarily large-step solvability is a separate issue for an [implicit Runge-Kutta method](../../../../../implicit-runge-kutta-method.md).

Order analysis has two levels: polynomial accuracy at stages and extra accuracy at the endpoint. Integration of interpolated powers gives the stage moment identities

$$
\sum_j a_{ij}c_j^{r-1}=\frac{c_i^r}{r},\qquad1\leq r\leq s.
$$

An induction in powers of $h$, using these identities in the stage equations, shows that the collocation polynomial agrees coefficientwise with the exact Taylor polynomial through degree $s$:

$$
U(\tau)=\sum_{r=0}^s\frac{h^r\tau^r}{r!}y^{(r)}(t_n)+O(h^{s+1}).
$$

For example, the coefficient of each new stage term is integrated exactly because its node dependence is a polynomial of degree at most $s-1$. This proves stage order $s$ and bounded actual-time derivatives of the collocation polynomial up to degree $s$. Assuming the vector field is sufficiently smooth on a fixed compact solution neighborhood, its composition with this polynomial has uniformly bounded derivatives of all finite orders needed below.

The endpoint weights define the interpolatory [quadrature rule](../../../../../quadrature-rule.md) $Q(v)=\sum_i b_i v(c_i)$. Suppose it is exact through degree $q-1$, but not through degree $q$. Necessarily $s\leq q\leq2s$: interpolation integrates degrees below $s$ exactly, while the nonzero polynomial $\omega(\tau)^2$, with $\omega(\tau)=\prod_i(\tau-c_i)$, has positive integral but quadrature value zero and degree $2s$. Exactness also implies the [nodal-polynomial criterion for quadrature exactness](../../../../../nodal-polynomial-criterion-for-quadrature-exactness.md)

$$
\int_0^1\omega(\tau)p(\tau)d\tau=0\quad\text{whenever }\deg p\leq q-s-1,
$$

because the integrand has degree at most $q-1$ and vanishes at every node.

Here is the endpoint-error argument underlying the [collocation order theorem](../../../../../collocation-order-theorem.md). Let $v(t)=U((t-t_n)/h)$ and $\delta(t)=v'(t)-f(t,v(t))$ be its residual. It vanishes at the collocation times, and if $F_h(\tau)=f(t_n+h\tau,U(\tau))$, then $\delta=\mathcal I_sF_h-F_h$, where $\mathcal I_s$ is interpolation at the nodes. Taylor expansion in actual time gives

$$
\delta(t_n+h\tau)=\sum_{r=s}^{q-1}h^r d_r\bigl(\mathcal I_s\tau^r-\tau^r\bigr)+O(h^q).
$$

The vector coefficients $d_r$ are bounded. Each bracket has the factor $\omega(\tau)$, with quotient degree $r-s$. In particular the residual is $O(h^s)$ throughout the step.

Write $\phi(t_*,t,z)$ for the exact flow from time $t$ and state $z$ to $t_*=t_n+h$. Differentiating $\phi(t_*,t,v(t))$ gives $D_z\phi(t_*,t,v(t))\delta(t)$: the derivative with respect to the starting time cancels the vector field by the flow composition identity. Integration therefore gives the exact local endpoint error

$$
v(t_*)-y(t_*)=\int_{t_n}^{t_*}\Psi(t)\delta(t)dt,\qquad\Psi(t)=D_z\phi(t_*,t,v(t)).
$$

For $q=s$, the $O(h^s)$ residual already gives $O(h^{s+1})$. For $q>s$, Taylor-expand the smooth matrix weight as $\Psi(t_n+h\tau)=\sum_{\ell=0}^{q-s-1}h^\ell\Psi_\ell\tau^\ell+O(h^{q-s})$. Every product term with $r+\ell<q$ integrates to zero: its polynomial factor is $\omega$ times a polynomial of degree $r-s+\ell\leq q-s-1$. All remaining terms are $O(h^q)$ before the time integration, including both remainders. Hence

$$
\boxed{\text{local endpoint error}=O(h^{q+1}),\qquad\text{global order}=q.}
$$

This is [collocation endpoint superconvergence by quadrature orthogonality](../../../../../collocation-endpoint-superconvergence-by-quadrature-orthogonality.md). For the global assertion, the stage contraction estimate gives a one-step Lipschitz bound $1+Ch$ on a fixed solution neighborhood. Thus the propagated error satisfies $e_{n+1}\leq(1+Ch)e_n+C h^{q+1}$, and the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md) gives $e_n=O(h^q)$ on a fixed time interval. The order cannot generically exceed $q$: for $y'=t^q$, each collocation step reduces to the same quadrature rule, whose first nonexact moment yields a nonzero $O(h^{q+1})$ local error and $O(h^q)$ composite error.

The usual node families illustrate the result. [Gauss collocation methods](../../../../../gauss-legendre-method.md) use interior Gaussian nodes and have $q=2s$, the maximum possible order. Right-endpoint Radau nodes give the [Radau IIA method](../../../../../radau-iia-method.md) of order $2s-1$. Including both endpoints with [Lobatto quadrature](../../../../../lobatto-quadrature.md) gives the [Lobatto IIIA method](../../../../../lobatto-iiia-method.md) of order $2s-2$ for $s\geq2$. One-stage Gaussian collocation is the second-order [implicit midpoint rule](../../../../../implicit-midpoint-rule.md), while collocation at the right endpoint is the first-order [Backward Euler method](../../../../../backward-euler-method.md). The two-stage Gaussian nodes $1/2\pm\sqrt3/6$ give $b=(1/2,1/2)$ and

$$
A=\begin{pmatrix}1/4&1/4-\sqrt3/6\\1/4+\sqrt3/6&1/4\end{pmatrix},
$$

a fourth-order method. Node placement, rather than just stage count, controls the superconvergent endpoint order.

There is also a structural link with Question 2. For Gaussian nodes, let $L_i(\tau)=\int_0^\tau\ell_i(v)dv$. The derivative of $L_iL_j$ has degree at most $2s-1$, so Gaussian quadrature is exact on it. The integral is $b_i b_j$, while evaluating at the nodes gives $b_i a_{ij}+b_j a_{ji}$. Thus Gaussian collocation satisfies $M=0$ and has [Runge-Kutta conservation of quadratic invariants](../../../../../runge-kutta-conservation-of-quadratic-invariants.md). For the scalar test equation, any [RK method](../../../../../runge-kutta-method.md) has [stability function](../../../../../stability-function.md) $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$. For implicit midpoint this is $(1+z/2)/(1-z/2)$; the identity $|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z$ proves [A-stability](../../../../../a-stability.md). High order, stage solvability, invariant preservation and damping are distinct design considerations, so no stability conclusion should be inferred from collocation order alone.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
