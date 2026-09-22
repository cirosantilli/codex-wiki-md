# Runge-Kutta method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Runge-Kutta_method)

A Runge-Kutta method advances an [initial value problem](differential-equation.md#initial-value-problem) $y'=f(t,y)$, $y(t_0)=y_0$, by sampling its [vector field](multivariable-calculus.md#vector-field) at several trial states within one time step. These samples are [Runge-Kutta stages](#runge-kutta-stage); a weighted combination of their slopes produces the next state. The construction improves on the single [tangent line](calculus.md#tangent-line) used by the [Euler method](numerical-analysis.md#euler-method) while requiring evaluations of $f$, rather than explicit higher [derivatives](calculus.md#derivative) of the solution. It applies to scalar equations and systems of [ordinary differential equations](differential-equation.md#ordinary-differential-equation) alike. The coefficient choices distinguish methods such as [Heun's method](#heun-s-method), the [classical fourth-order Runge-Kutta method](#classical-fourth-order-runge-kutta-method) and [implicit Runge-Kutta methods](#implicit-runge-kutta-method).

For $s$ stages, write $A=(a_{ij})$ for the stage [matrix](vector-space.md#matrix), $c_i$ for relative time nodes and $b_i$ for output weights. A time step of length $h$ computes

$$
Y_i=y_n+h\sum_{j=1}^s a_{ij}k_j,\qquad k_i=f(t_n+c_i h,Y_i),\qquad y_{n+1}=y_n+h\sum_{i=1}^s b_i k_i.
$$

Here $k_i$ is a slope, with units of state per time; $hk_i$ is a state increment. Another common convention writes $K_i=hk_i$, so its stage states are $Y_i=y_n+\sum_j a_{ij}K_j$ and its output is $y_n+\sum_i b_iK_i$. These are equivalent conventions: including $h$ both inside $K_i$ and again in the output would count the time step twice. The textbook formulation uses the increment convention.[Fundamentals of Numerical Computation, §6.4.3, equations 6.4.10–6.4.11: multistage recipe and tableau](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/6-4-runge-kutta-methods)

Usually the [Butcher tableau](#butcher-tableau) obeys $c_i=\sum_ja_{ij}$, called internal consistency. Stage $i$ then combines slopes over an effective time $c_i h$. The [second-order conditions with independent Runge-Kutta abscissae](#second-order-conditions-with-independent-runge-kutta-abscissae) explain what changes when time nodes are specified independently. A [Runge-Kutta stage](#runge-kutta-stage) is generally an auxiliary approximation, not a separate accepted solution value at its node. Several stages can even have the same time node but different state arguments, as in the [classical fourth-order Runge-Kutta method](#classical-fourth-order-runge-kutta-method).

The useful idea is to approximate the [integral](integral.md) $y(t_n+h)-y(t_n)=\int_{t_n}^{t_n+h}f(t,y(t))\,dt$ without knowing the intermediate exact trajectory. Trial states provide places to sample $f$, and [Butcher order conditions](#butcher-order-condition) make the resulting combination agree with the exact [Taylor expansion](calculus.md#taylor-expansion). More stages alone do not guarantee a higher [order of a numerical method](numerical-analysis.md#order-of-a-numerical-method): their coefficients must satisfy the appropriate conditions. [Embedded Runge-Kutta pairs](error-control-for-ode-solvers.md#embedded-runge-kutta-pair) reuse these same samples for a second output and a practical [local error estimator](error-control-for-ode-solvers.md#local-error-estimator).

**Table of contents**

- [Runge-Kutta stage](#runge-kutta-stage)
- [Explicit Runge-Kutta method](#explicit-runge-kutta-method)
  - [Heun's method](#heun-s-method)
- [Maximal-order Runge-Kutta methods are A-stable](#maximal-order-runge-kutta-methods-are-a-stable)
- [Theta method](#theta-method)
  - [Theta diffusion stability criterion](#theta-diffusion-stability-criterion)
    - [Rough-data damping distinction for the theta method](#rough-data-damping-distinction-for-the-theta-method)
- [Strong stability preserving Runge-Kutta method](#strong-stability-preserving-runge-kutta-method)
- [Classical fourth-order Runge-Kutta method](#classical-fourth-order-runge-kutta-method)
- [Butcher tableau](#butcher-tableau)
- [Butcher order condition](#butcher-order-condition)
  - [Second-order conditions with independent Runge-Kutta abscissae](#second-order-conditions-with-independent-runge-kutta-abscissae)
  - [Fourth-order conditions for a Runge-Kutta method](#fourth-order-conditions-for-a-runge-kutta-method)
- [Implicit Runge-Kutta method](#implicit-runge-kutta-method)
  - [Two-stage Runge-Kutta family with an implicit second stage](#two-stage-runge-kutta-family-with-an-implicit-second-stage)
  - [Stage solvability of an implicit Runge-Kutta method](#stage-solvability-of-an-implicit-runge-kutta-method)
  - [Implicit midpoint rule](#implicit-midpoint-rule)
  - [Crank-Nicolson method](#crank-nicolson-method)
    - [Contractivity of split Crank-Nicolson diffusion](#contractivity-of-split-crank-nicolson-diffusion)
  - [Collocation Runge-Kutta method](#collocation-runge-kutta-method)
    - [Two-node collocation A-stability criterion](#two-node-collocation-a-stability-criterion)
    - [Collocation order theorem](#collocation-order-theorem)
      - [Collocation endpoint superconvergence by quadrature orthogonality](#collocation-endpoint-superconvergence-by-quadrature-orthogonality)
    - [Collocation tableau row-sum identity](#collocation-tableau-row-sum-identity)
    - [Lobatto IIIA method](#lobatto-iiia-method)
    - [Gauss-Legendre method](#gauss-legendre-method)
      - [Gauss collocation coefficient construction](#gauss-collocation-coefficient-construction)
      - [Fourth-order two-stage Gauss collocation method](#fourth-order-two-stage-gauss-collocation-method)
    - [Radau IIA method](#radau-iia-method)
      - [Padé identification of a Radau stability function](#pade-identification-of-a-radau-stability-function)
    - [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)
      - [Runge-Kutta conservation of quadratic invariants](#runge-kutta-conservation-of-quadratic-invariants)
      - [Butcher contractivity theorem](#butcher-contractivity-theorem)
      - [Runge-Kutta contractivity identity](#runge-kutta-contractivity-identity)
  - [Trapezoidal rule](#trapezoidal-rule)
    - [Composite trapezoidal rule](#composite-trapezoidal-rule)
    - [Trapezoidal rule fails B-stability](#trapezoidal-rule-fails-b-stability)
- [Time-symmetric numerical method](#time-symmetric-numerical-method)
- [Order of a Runge-Kutta method](#order-of-a-runge-kutta-method)
  - [Third-order conditions for an explicit Runge-Kutta method](#third-order-conditions-for-an-explicit-runge-kutta-method)

## Runge-Kutta stage

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

A Runge-Kutta stage consists of a trial state $Y_i$ at the time node $t_n+c_i h$ and the corresponding [vector field](multivariable-calculus.md#vector-field) evaluation $k_i$. In the slope convention, $Y_i=y_n+h\sum_ja_{ij}k_j$. Stages belong to the construction of one [Runge-Kutta method](runge-kutta-method.md) step; they need not have the same accuracy as its final output. Stage states can leave the physically allowed region even when the endpoint lies inside it, so $f$ must be defined at every stage used.

## Explicit Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

An explicit Runge-Kutta method has $a_{ij}=0$ whenever $j\geq i$. Its stage [matrix](vector-space.md#matrix) is strictly lower triangular: compute each [Runge-Kutta stage](#runge-kutta-stage) using already known slopes, starting with $Y_1=y_n$. In contrast, an [implicit Runge-Kutta method](#implicit-runge-kutta-method) requires solving coupled stage equations, whose existence is addressed by [stage solvability of an implicit Runge-Kutta method](#stage-solvability-of-an-implicit-runge-kutta-method).

<h3 id="heun-s-method">Heun's method</h3>

↑ **Parent:** [Explicit Runge-Kutta method](#explicit-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heun's_method)

Here Heun's method means the explicit endpoint-averaging [Runge-Kutta method](runge-kutta-method.md): take an Euler predictor $Y_2=y_n+hf(t_n,y_n)$, sample $k_2=f(t_n+h,Y_2)$ there, and average it with $k_1=f(t_n,y_n)$ for the output. The second [Runge-Kutta stage](#runge-kutta-stage) is evaluated at the predictor, not at the corrected endpoint. In particular it requires no implicit solve as the ODE [trapezoidal rule](#trapezoidal-rule) does. Naming conventions vary between books; the formulas specify the method unambiguously.[André Massing, Numerical solution of ordinary differential equations: One step methods, October 3, 2021, page 1, Example 1.1: Euler and Heun increment functions](mathematics-bibliography.md#numerical-solution-of-ordinary-differential-equations-one-step-methods-by-andre-jurgen-massing)

For smooth $f$, a [Taylor expansion](calculus.md#taylor-expansion) about $(t_n,y_n)$ gives $k_2=f+h(f_t+f_yf)+O(h^2)$, where $f_y$ is the state [Jacobian matrix](multivariable-calculus.md#jacobian-matrix). Consequently the output is $y_n+hf+h^2(f_t+f_yf)/2+O(h^3)$, matching the exact solution through degree two by the [chain rule](calculus.md#chain-rule). This gives [local truncation error](numerical-analysis.md#local-truncation-error) $O(h^3)$ and, with the usual bounded smoothness and [Lipschitz continuity](real-analysis.md#lipschitz-continuity) hypotheses on a fixed finite interval, [global error](numerical-analysis.md#global-discretization-error) $O(h^2)$. The [Euler-Heun embedded pair](error-control-for-ode-solvers.md#euler-heun-embedded-pair) compares this output with its Euler predictor.

<a id="image-euler-heun-stage-geometry-for-y-prime-equals-y-sample-at-the-euler-predictor-then-average-slopes-for-the-corrected-endpoint"></a>
![](euler-heun-slopes-and-stage-construction.png)

**[Figure 1](#image-euler-heun-stage-geometry-for-y-prime-equals-y-sample-at-the-euler-predictor-then-average-slopes-for-the-corrected-endpoint). Euler-Heun stage geometry for y prime equals y: sample at the Euler predictor, then average slopes for the corrected endpoint**.

For $y'=y$, $y_n=1$ and $h=0.2$, the sampled slopes are $1$ and $1.2$. Transporting the second slope to the starting point would end at $1.24$; the average slope $1.1$ instead ends at $1.22$. The exact [exponential function](calculus.md#exponential-function) reaches $e^{0.2}\approx1.22140275816$. The magnified endpoint comparison separates the pair difference $0.02$ from the actual Heun local defect $0.00140275816$.

## Maximal-order Runge-Kutta methods are A-stable

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

An $s$-stage [Runge-Kutta method](runge-kutta-method.md) has [stability function](numerical-analysis.md#stability-function) $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$, a [rational function](isolated-singularity.md#rational-function) with numerator and denominator degrees at most $s$. Order $2s$ forces $R(z)-e^z=O(z^{2s+1})$, so uniqueness of the diagonal [Padé approximant](isolated-singularity.md#pade-approximant) identifies $R$ with $[s/s]_{e^z}$. That approximant has no poles in the closed left half-plane and modulus at most one there. Hence every such maximal-order method is [A-stable](numerical-analysis.md#a-stability). Since the [Padé approximant](isolated-singularity.md#pade-approximant) numerator and denominator are coprime and both have degree $s$, the original stage [determinant](multilinear-algebra.md#determinant) cannot have hidden canceled poles in that half-plane.

## Theta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

This one-step family interpolates between the [Forward Euler method](numerical-analysis.md#euler-method) at $a=0$, the [trapezoidal rule](#trapezoidal-rule) at $a=1/2$, and the [Backward Euler method](numerical-analysis.md#backward-euler-method) at $a=1$. Its [stability function](numerical-analysis.md#stability-function) is $R(z)=[1+(1-a)z]/[1-az]$. It is first order except at one half, where it is second order. Applying it to spatial diffusion gives the [theta diffusion stability criterion](#theta-diffusion-stability-criterion).

### Theta diffusion stability criterion

↑ **Parent:** [Theta method](#theta-method)

On an orthogonal diffusion eigenmode, the [theta method](#theta-method) has the displayed amplification with $s=-\Delta t\lambda$. The identity $(1+as)^2-[1-(1-a)s]^2=2s+(2a-1)s^2$ proves contraction at all nonnegative $s$ exactly when $a\geq1/2$. For $a<1/2$, contraction holds up to $s\leq2/(1-2a)$, with a positive denominator in that range. Orthogonality is what transfers these modal bounds to a full [L2 norm](real-analysis.md#l2-norm) estimate.

#### Rough-data damping distinction for the theta method

↑ **Parent:** [Theta diffusion stability criterion](#theta-diffusion-stability-criterion)

At $a=1/2$, arbitrarily stiff heat modes approach amplification $-1$: the [Crank-Nicolson method](#crank-nicolson-method) is contractive but does not rapidly damp unresolved rough components. The [Backward Euler method](numerical-analysis.md#backward-euler-method) instead has limit zero. Thus unconditional linear stability and strong stiff decay are different requirements. High smooth-data consistency order alone does not imply a uniform high-order estimate down to the initial instant for arbitrary [L2 initial conditions](differential-equation.md#l2-initial-condition).

## Strong stability preserving Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

A strong stability preserving Runge-Kutta method writes its stages as convex combinations of previously computed states and suitable [Forward Euler method](numerical-analysis.md#euler-method) steps. It transfers any convex-functional nonincrease property of the forward step, such as a [norm](normed-vector-space.md#norm) bound, under a proportionally scaled time-step restriction.

For example, if $E_k(U)=U+kF(U)$ is nonexpansive in a [norm](normed-vector-space.md#norm), then $Y=E_k(U)$ and $U_{\mathrm{new}}=(U+E_k(Y))/2$ is also nonexpansive: the [triangle inequality](topological-analysis.md#triangle-inequality) bounds the new difference by one half of the initial difference plus one half of the twice-advanced difference. Both are at most the initial difference. A [Taylor expansion](calculus.md#taylor-expansion) yields $U_{\mathrm{new}}=U+kF(U)+k^2F'(U)F(U)/2+O(k^3)$, so this is a second-order [Runge-Kutta method](runge-kutta-method.md). The forward-step hypothesis must hold on the stage states; preservation of one chosen convex bound is not the same as unconditional [B-stability](numerical-analysis.md#b-stability).

## Classical fourth-order Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

The classical four-stage explicit [Runge-Kutta method](runge-kutta-method.md) uses

$$
A=\begin{pmatrix}0&0&0&0\\1/2&0&0&0\\0&1/2&0&0\\0&0&1&0\end{pmatrix},\qquad
b=(1/6,1/3,1/3,1/6)^T,\qquad c=(0,1/2,1/2,1)^T.
$$

It satisfies the [fourth-order conditions for a Runge-Kutta method](#fourth-order-conditions-for-a-runge-kutta-method). Its polynomial [stability function](numerical-analysis.md#stability-function) excludes [A-stability](numerical-analysis.md#a-stability), while $|R(iq)|^2=1-q^6/72+q^8/576$ gives the imaginary-axis stability interval $|q|\leq2\sqrt2$.

## Butcher tableau

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

A Butcher tableau records a [Runge-Kutta method](runge-kutta-method.md)'s stage [matrix](vector-space.md#matrix) $A$, time nodes $c$, and output weights $b$ in the block array

$$
\begin{array}{c|c}c&A\\\hline&b^T\end{array}.
$$

Read row $i$ above the line as the recipe for [Runge-Kutta stage](#runge-kutta-stage) $i$: the left entry gives $t_n+c_i h$, and the right entries give the coefficients in $Y_i=y_n+h\sum_ja_{ij}k_j$. Below the line, $b_i$ weights slope $k_i$ in the final update. Zeros on and above the diagonal identify an [Explicit Runge-Kutta method](#explicit-runge-kutta-method). For the internally consistent convention, row sums of $A$ equal $c$; first-order [consistency of a numerical method](numerical-analysis.md#consistency-of-a-numerical-method) also requires $\sum_i b_i=1$. An [embedded Runge-Kutta pair](error-control-for-ode-solvers.md#embedded-runge-kutta-pair) adds another weight row while retaining $A,c$.

## Butcher order condition

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

A Butcher order condition equates the coefficient assigned by a [Runge-Kutta method](runge-kutta-method.md) to a rooted tree with the corresponding exact Taylor coefficient. Satisfying every condition through tree order $p$ is equivalent to Runge–Kutta order at least $p$.

### Second-order conditions with independent Runge-Kutta abscissae

↑ **Parent:** [Butcher order condition](#butcher-order-condition)

For a general nonautonomous [Runge-Kutta method](runge-kutta-method.md), [Taylor expansion](calculus.md#taylor-expansion) of stage $i$ gives $k_i=f+h[c_if_t+(Ae)_if_yf]+O(h^2)$. Matching the exact increment $hf+h^2(f_t+f_yf)/2$ gives the three displayed conditions. When internal consistency $c=Ae$ is imposed, the last two coincide. Internal consistency is a usual tableau convention, but is not logically necessary for order two of a generalized tableau.

### Fourth-order conditions for a Runge-Kutta method

↑ **Parent:** [Butcher order condition](#butcher-order-condition)

With $c=Ae$ and $C=\operatorname{diag}(c)$, a [Runge-Kutta method](runge-kutta-method.md) has order at least four exactly when the eight [Butcher order conditions](#butcher-order-condition)

$$
b^Te=1,\quad b^Tc=\frac12,\quad b^Tc^2=\frac13,\quad b^TAc=\frac16,\quad b^Tc^3=\frac14,\quad b^TCAc=\frac18,\quad b^TAc^2=\frac1{12},\quad b^TA^2c=\frac1{24}
$$

hold; powers of $c$ are componentwise. These conditions match the numerical and exact coefficients indexed by [rooted trees](tree-graph-theory.md#rooted-tree) through order four. Matching the scalar [Dahlquist test equation](numerical-analysis.md#dahlquist-test-equation) alone is insufficient to check the nonlinear [Butcher order conditions](#butcher-order-condition).

## Implicit Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_Runge-Kutta_method)

An implicit Runge-Kutta method defines one or more stages through equations involving those same stages.

### Two-stage Runge-Kutta family with an implicit second stage

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

For stages $k_1=f(y)$ and $k_2=f(y+(1-a)hk_1+ahk_2)$ with update $y+h(k_1+k_2)/2$, the method has order two for every fixed real $a$. The third-order coefficient of $f''f^2$ is always $1/4$, not $1/6$, so no parameter gives third order on general nonlinear equations. The displayed [stability function](numerical-analysis.md#stability-function) is bounded throughout the left half-plane only when $a=1/2$, when it is the A-stable trapezoidal function $(1+z/2)/(1-z/2)$. It is not L-stable.

### Stage solvability of an implicit Runge-Kutta method

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

For a vector field uniformly [Lipschitz continuous](real-analysis.md#lipschitz-continuity) in the state with constant $L$, the stage fixed-point map of an [implicit Runge-Kutta method](#implicit-runge-kutta-method) is a contraction in the maximum stage norm if $hL\max_i\sum_j|a_{ij}|<1$. The [contraction mapping theorem](analysis.md#contraction-mapping-theorem) then gives unique stages. This is a sufficient small-step condition; a [dissipative vector field](differential-equation.md#dissipative-vector-field) may permit solvability for larger steps. An [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) or [B-stability](numerical-analysis.md#b-stability) estimate compares existing stage solutions and should not be mistaken for an unqualified stage-existence theorem.

### Implicit midpoint rule

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

The implicit midpoint rule advances an autonomous ordinary differential equation by

$$
y_{n+1}=y_n+h f\left(\frac{y_n+y_{n+1}}2\right).
$$

It is a second-order, [A-stable](numerical-analysis.md#a-stability), [time-symmetric numerical method](#time-symmetric-numerical-method).

The [implicit midpoint rule](#implicit-midpoint-rule) is the [midpoint method](numerical-analysis.md#midpoint-method) with $y_{n+1}=y_n+h f(t_n+h/2,(y_n+y_{n+1})/2)$. It is a one-stage [implicit Runge-Kutta method](#implicit-runge-kutta-method).

### Crank-Nicolson method

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crank–Nicolson_method)

The Crank--Nicolson method applies the [trapezoidal rule](#trapezoidal-rule) to a semidiscrete evolution equation. For a linear system $u'=Lu$ its update is

$$
\left(I-\frac h2L\right)u^{n+1}=\left(I+\frac h2L\right)u^n.
$$

#### Contractivity of split Crank-Nicolson diffusion

↑ **Parent:** [Crank-Nicolson method](#crank-nicolson-method)

For symmetric negative semidefinite matrices $A,B$, each factor $C_A(h)=(I-hA/2)^{-1}(I+hA/2)$ has norm at most one, since its eigenvalues are $(1+h\lambda/2)/(1-h\lambda/2)$ with $\lambda\le0$. The same holds for $B$, so their ordered product is a contraction for every $h\ge0$, whether or not $A,B$ commute. This proves unconditional discrete [L2 norm](real-analysis.md#l2-norm) stability of the split [Crank-Nicolson method](#crank-nicolson-method) for directional diffusion. Its splitting error remains first order in general, because the product's quadratic defect is $h^2[A,B]/2$.

### Collocation Runge-Kutta method

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

Given distinct nodes $c_i$, a collocation Runge-Kutta method uses the Lagrange basis $\ell_j$ with $a_{ij}=\int_0^{c_i}\ell_j(\tau)d\tau$ and $b_j=\int_0^1\ell_j(\tau)d\tau$. Its stages enforce the differential equation at the collocation nodes.

This applies the [collocation method](numerical-analysis.md#collocation-method) to the time-step polynomial of an [ordinary differential equation](differential-equation.md#ordinary-differential-equation).

#### Two-node collocation A-stability criterion

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

For distinct nodes $c_1,c_2\in[0,1]$, the two-stage [collocation Runge-Kutta method](#collocation-runge-kutta-method) has [stability function](numerical-analysis.md#stability-function)

$$
R(z)=\frac{1+(1-a)z+rz^2}{1-az+dz^2},\qquad a=(c_1+c_2)/2,\quad d=c_1c_2/2,\quad r=(1-c_1)(1-c_2)/2.
$$

The denominator has no zeros in the closed left half-plane. On the imaginary axis the denominator's squared modulus minus the numerator's is $(d^2-r^2)y^4$. Thus $d\geq r$, equivalently $c_1+c_2\geq1$, is necessary and sufficient for [A-stability](numerical-analysis.md#a-stability), using the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle) and the bound at infinity.

#### Collocation order theorem

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

For $s$ distinct collocation nodes, let $\pi_s(t)=\prod_{i=1}^s(t-c_i)$. If $\int_0^1t^j\pi_s(t)dt=0$ for $0\le j<k$, and the next moment is nonzero, the associated interpolatory quadrature has order $s+k$, and the [collocation Runge-Kutta method](#collocation-runge-kutta-method) has the same classical order for sufficiently smooth differential equations. Here $0\le k\le s$. Equivalently, if the quadrature is exact through degree $p-1$ but not degree $p$, the method has order $p$. The generic order is at least $s$, [Gauss collocation methods](#gauss-legendre-method) reach $2s$, and [Radau IIA methods](#radau-iia-method) reach $2s-1$.

##### Collocation endpoint superconvergence by quadrature orthogonality

↑ **Parent:** [Collocation order theorem](#collocation-order-theorem)

For $s$ collocation nodes, the residual of the collocation polynomial vanishes at each node and contains the factor $\omega(\tau)=\prod_i(\tau-c_i)$. Quadrature exactness through degree $q-1$ implies $\int_0^1\omega(\tau)p(\tau)d\tau=0$ for every polynomial of degree at most $q-s-1$. Expand the smooth vector-field interpolation error and the derivative of the exact flow in powers of the step. Every endpoint-error term of degree below $q$ has this vanishing weighted moment, so the endpoint local error is $O(h^{q+1})$, although the interior stage accuracy is generally only $s$. A step Lipschitz estimate and [discrete Gronwall inequality](probability-and-statistics.md#discrete-gronwall-inequality) then give global order $q$. Gaussian nodes attain $q=2s$, while the first nonexact quadrature moment bounds the order from above.

#### Collocation tableau row-sum identity

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

For a [collocation Runge-Kutta method](#collocation-runge-kutta-method), $a_{ij}=\int_0^{c_i}\ell_j(t)dt$, where the [Lagrange interpolation](interpolation.md#lagrange-polynomial) basis obeys $\sum_j\ell_j=1$. Hence each row sum is its collocation node. Failure of this identity disproves a claimed collocation tableau with those nodes. The identity alone is necessary rather than sufficient: the individual integrated basis coefficients must also agree.

#### Lobatto IIIA method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

A Lobatto IIIA method collocates at the [Lobatto quadrature](numerical-analysis.md#lobatto-quadrature) nodes, including both endpoints of the time interval. Its three-stage version has

$$
A=\begin{pmatrix}0&0&0\\5/24&1/3&-1/24\\1/6&2/3&1/6\end{pmatrix},
\qquad b=(1/6,2/3,1/6)^T,
\qquad c=(0,1/2,1)^T.
$$

The [Butcher order conditions](#butcher-order-condition) give order four. Its [stability function](numerical-analysis.md#stability-function) is

$$
R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12},
$$

which is [A-stable](numerical-analysis.md#a-stability) but not [L-stable](numerical-analysis.md#l-stability). It is not [algebraically stable](#algebraic-stability-of-a-runge-kutta-method): the first diagonal entry of the defining [matrix](vector-space.md#matrix) is $2b_1a_{11}-b_1^2=-1/36$. This distinguishes linear [A-stability](numerical-analysis.md#a-stability) from nonlinear [algebraic stability](#algebraic-stability-of-a-runge-kutta-method).

#### Gauss-Legendre method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Legendre_method)

The $s$-stage Gauss--Legendre Runge--Kutta method collocates at the Gauss--Legendre quadrature nodes on $[0,1]$. It is symmetric, A-stable, and has order $2s$.

##### Gauss collocation coefficient construction

↑ **Parent:** [Gauss-Legendre method](#gauss-legendre-method)

Choose $c_1,\ldots,c_s$ as the [polynomial roots](polynomial.md#root-of-a-polynomial) of $P_s(2c-1)$ in $(0,1)$, and form the [Lagrange interpolation polynomials](interpolation.md#lagrange-polynomial) $\ell_j(t)=\prod_{m\ne j}(t-c_m)/(c_j-c_m)$. The [Gauss collocation method](#gauss-legendre-method) has $a_{ij}=\int_0^{c_i}\ell_j(t)dt$ and $b_j=\int_0^1\ell_j(t)dt$. This gives explicit coefficient formulas after finding [polynomial roots](polynomial.md#root-of-a-polynomial): if $\ell_j(t)=\sum_rd_{jr}t^r$, these [integrals](integral.md) are $\sum_rd_{jr}c_i^{r+1}/(r+1)$ and $\sum_rd_{jr}/(r+1)$. [Gaussian quadrature](numerical-analysis.md#gaussian-quadrature) gives order $2s$.

##### Fourth-order two-stage Gauss collocation method

↑ **Parent:** [Gauss-Legendre method](#gauss-legendre-method)

The two-stage [Gauss--Legendre Runge-Kutta method](#gauss-legendre-method) uses nodes $c_{1,2}=1/2\mp\sqrt3/6$, weights $b_1=b_2=1/2$ and coefficients $a_{11}=a_{22}=1/4$, $a_{12}=1/4-\sqrt3/6$, $a_{21}=1/4+\sqrt3/6$. The [Butcher order conditions](#butcher-order-condition) give order four. Its [stability function](numerical-analysis.md#stability-function) is the displayed rational function, which is [A-stable](numerical-analysis.md#a-stability). The [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) matrix is zero, so positive weights also give nonlinear contractivity for dissipative vector fields.

#### Radau IIA method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

An $s$-stage Radau IIA method collocates at the right-endpoint Radau nodes. It has order $2s-1$ and is both [algebraically stable](#algebraic-stability-of-a-runge-kutta-method) and [L-stable](numerical-analysis.md#l-stability).

<h5 id="pade-identification-of-a-radau-stability-function">Padé identification of a Radau stability function</h5>

↑ **Parent:** [Radau IIA method](#radau-iia-method)

Suppose an $s$-stage [Runge-Kutta method](runge-kutta-method.md) has order $2s-1$, an [invertible matrix](linear-algebra.md#invertible-matrix) $A$, and $b^TA^{-1}\mathbf1=1$. Its [stability function](numerical-analysis.md#stability-function) is $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$. The [adjugate matrix](linear-algebra.md#adjugate-matrix) formula gives a [rational function](isolated-singularity.md#rational-function) with denominator degree $s$ and numerator degree at most $s$; its zero [limit](calculus.md#limit-of-a-function) at infinity lowers the latter degree to at most $s-1$. The [order of a numerical method](numerical-analysis.md#order-of-a-numerical-method) gives $R(z)-e^z=O(z^{2s})$, identifying the $[s-1/s]$ [Padé approximant](isolated-singularity.md#pade-approximant). Uniqueness follows because the cross-multiplied difference of two candidates has degree at most $2s-1$ but a zero of order at least $2s$, so is identically zero. The [A-stability of near-diagonal exponential Padé approximants](numerical-analysis.md#a-stability-of-near-diagonal-exponential-pade-approximants) then proves [A-stability](numerical-analysis.md#a-stability), and the zero limit proves [L-stability](numerical-analysis.md#l-stability). These conditions identify the stability function; they do not alone claim uniqueness of all entries of the [Runge-Kutta method](runge-kutta-method.md) tableau.

#### Algebraic stability of a Runge-Kutta method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

A Runge-Kutta method is algebraically stable when $b_i\geq0$ and the matrix $M$ with $M_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j$ is positive semidefinite. Algebraic stability implies contractivity for dissipative differential equations.

##### Runge-Kutta conservation of quadratic invariants

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)

For stage states $Y_i=y_n+h\sum_ja_{ij}k_j$ and a vector field with $Y_i^Tk_i=0$, expansion of the new squared norm gives $\|y_{n+1}\|^2-\|y_n\|^2=-h^2\sum_{i,j}M_{ij}k_i^Tk_j$, where $M_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j$. Hence $M=0$ preserves the [quadratic form](quadratic-form.md) exactly for every well-defined step. The same argument with a fixed symmetric matrix in the inner product preserves any quadratic invariant of the vector field. In particular it preserves the Euclidean norm for a [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix) differential equation.

##### Butcher contractivity theorem

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)

An [algebraically stable](#algebraic-stability-of-a-runge-kutta-method) [Runge-Kutta method](runge-kutta-method.md) is [B-stable](numerical-analysis.md#b-stability): for a [dissipative vector field](differential-equation.md#dissipative-vector-field), a well-defined step cannot increase the distance between two starting values. This assumes that the compared stage equations have solutions, as required by [stage solvability of an implicit Runge-Kutta method](#stage-solvability-of-an-implicit-runge-kutta-method). The [Runge-Kutta contractivity identity](#runge-kutta-contractivity-identity) expresses the distance change as a nonpositive weighted term coming from the [dissipative vector field](differential-equation.md#dissipative-vector-field) minus a nonnegative [quadratic form](quadratic-form.md) involving the matrix defining [algebraic stability](#algebraic-stability-of-a-runge-kutta-method). Positive weights also rule out stage poles in the open left half-plane on the scalar test equation, giving [A-stability](numerical-analysis.md#a-stability) there; zero-weight redundant stages need separate solvability attention.

##### Runge-Kutta contractivity identity

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)

For differences $D_i$ between corresponding stages and differences $F_i$ between their vector fields, a Runge--Kutta step satisfies

$$
\|d_{n+1}\|^2=\|d_n\|^2+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

To derive the identity, expand the squared [norm](normed-vector-space.md#norm) of $d_{n+1}=d_n+h\sum_i b_iF_i$ and substitute $d_n=D_i-h\sum_j a_{ij}F_j$ in the linear term. Symmetrizing the double sum gives the displayed coefficients $m_{ij}$. For a [dissipative vector field](differential-equation.md#dissipative-vector-field), the first sum is nonpositive when $b_i\geq0$, and the second sum is nonnegative when the [matrix](vector-space.md#matrix) $(m_{ij})$ is a [positive semidefinite matrix](quadratic-form.md#positive-semidefinite-matrix). Thus [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) implies [B-stability](numerical-analysis.md#b-stability).

### Trapezoidal rule

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trapezoidal_rule)

As a [quadrature rule](numerical-integration.md#quadrature-rule), the [trapezoidal rule](#trapezoidal-rule) replaces an [integrand](integral.md#integrand) by the [linear interpolation](function.md#linear-interpolation) joining its two endpoint values:

$$
I(f)=\int_a^bf(x)\,dx\approx T(f)=\frac{b-a}{2}\bigl(f(a)+f(b)\bigr),\qquad a<b.
$$

For nonnegative endpoint values, this is the area of a [trapezoid](euclidean-geometry.md#trapezoid); in general it is a signed area. The [quadrature nodes](numerical-integration.md#quadrature-node) are $a,b$, each with [quadrature weight](numerical-integration.md#quadrature-weight) $(b-a)/2$. Unlike the [midpoint quadrature rule](numerical-analysis.md#midpoint-quadrature-rule), it uses endpoint samples, which can be reused between adjacent panels.

Every [affine function](vector-space.md#affine-function) $f(x)=\alpha x+\beta$ agrees with its [linear interpolation](function.md#linear-interpolation), so the [trapezoidal rule](#trapezoidal-rule) integrates it exactly. On $[0,2]$, $f(x)=2x+1$ gives $T(f)=(2/2)(1+5)=6=I(f)$. On $[0,1]$, the [polynomial](polynomial.md) $f(x)=x^2$ instead gives $T(f)=1/2$, exceeding $I(f)=1/3$ by $1/6$. Its [degree of precision of a quadrature rule](numerical-integration.md#degree-of-precision-of-a-quadrature-rule) is exactly one.

If $f\in C^2[a,b]$, its signed [approximation error](numerical-analysis.md#approximation-error) satisfies

$$
T(f)-I(f)=\frac{(b-a)^3}{12}f''(\xi_T),\qquad a<\xi_T<b.
$$

A [convex function](real-analysis.md#convex-function) lies below its endpoint chord, so the [trapezoidal rule](#trapezoidal-rule) overestimates its [integral](integral.md); a [concave function](real-analysis.md#concave-function) gives the reverse inequality. The error formula assumes that the second [derivative](calculus.md#derivative) exists and is a [continuous function](calculus.md#continuous-function) throughout the closed interval.[§3.5(i), equation 3.5.1 and its C² hypothesis; the source writes integral minus rule](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-i-trapezoidal-rules) A short derivation is the identity

$$
T(f)-I(f)=\frac12\int_a^b(t-a)(b-t)f''(t)\,dt,
$$

obtained by two [integrations by parts](calculus.md#integration-by-parts). The nonnegative [Peano kernel](numerical-analysis.md#peano-kernel) has [integral](integral.md) $(b-a)^3/12$, and the [weighted mean value theorem for integrals](real-analysis.md#weighted-mean-value-theorem-for-integrals) gives the formula.

The [trapezoidal rule](#trapezoidal-rule) for an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) averages [vector fields](multivariable-calculus.md#vector-field) at the old and new states and is [A-stable](numerical-analysis.md#a-stability).

This time-stepping use applies the same [trapezoidal rule](#trapezoidal-rule) to the [integral](integral.md) of the [derivative](calculus.md#derivative) in an [ordinary differential equation](differential-equation.md#ordinary-differential-equation). That connection explains its place under [implicit Runge-Kutta methods](#implicit-runge-kutta-method); its quadrature behavior and the nonlinear issue in [trapezoidal rule fails B-stability](#trapezoidal-rule-fails-b-stability) concern different uses of the same endpoint averaging.

#### Composite trapezoidal rule

↑ **Parent:** [Trapezoidal rule](#trapezoidal-rule)

On an equal-panel [partition of an interval](real-analysis.md#partition-of-an-interval), with $h=(b-a)/n$, sum the [trapezoidal rule](#trapezoidal-rule) over adjacent panels:

$$
T_n(f)=h\left[\frac{f(a)}2+\sum_{j=1}^{n-1}f(a+jh)+\frac{f(b)}2\right].
$$

There are $n+1$ distinct [quadrature nodes](numerical-integration.md#quadrature-node). Each interior sample belongs to two panels and therefore has [quadrature weight](numerical-integration.md#quadrature-weight) $h$, while each endpoint has [quadrature weight](numerical-integration.md#quadrature-weight) $h/2$. Equivalently, the [composite trapezoidal rule](#composite-trapezoidal-rule) integrates the [piecewise linear function](function.md#piecewise-linear-function) obtained by [linear interpolation](function.md#linear-interpolation) exactly.[§5.6.1, equations 5.6.3–5.6.5: integrating the piecewise linear interpolant](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/5-6-numerical-integration)

For $f\in C^2[a,b]$ and $K=\max_{x\in[a,b]}|f''(x)|$, summing panel [quadrature errors](real-analysis.md#quadrature-error) gives

$$
T_n(f)-I(f)=\frac{b-a}{12}h^2f''(\xi),\qquad |T_n(f)-I(f)|\leq\frac{b-a}{12}h^2K
$$

for some $\xi\in(a,b)$. Thus panel [quadrature errors](real-analysis.md#quadrature-error) of order $O(h^3)$ accumulate to order $O(h^2)$, using [big O notation](real-analysis.md#big-o-notation).[§3.5(i), equations 3.5.2–3.5.3: composite formula and signed error](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-i-trapezoidal-rules) On a nonuniform [partition of an interval](real-analysis.md#partition-of-an-interval) with widths $h_j$ and largest width $H$, the bound is $K\sum_jh_j^3/12\leq K(b-a)H^2/12$.

For the [polynomial](polynomial.md) $f(x)=x^2$ on $[0,1]$, direct summation yields

$$
T_n(f)=\frac13+\frac{1}{6n^2},\qquad T_n(f)-I(f)=-2\bigl(M_n(f)-I(f)\bigr).
$$

Both [quadrature errors](real-analysis.md#quadrature-error) shrink by exactly four when $n$ doubles, with opposite signs. This exact relation belongs to this [polynomial](polynomial.md) example; the [trapezoidal rule](#trapezoidal-rule) is not always twice as inaccurate as the [midpoint quadrature rule](numerical-analysis.md#midpoint-quadrature-rule).

<a id="image-quadratic-quadrature-errors-fall-by-four-on-refinement-while-a-common-sample-bias-persists"></a>
![](midpoint-trapezoidal-error-refinement.png)

**[Figure 2](#image-quadratic-quadrature-errors-fall-by-four-on-refinement-while-a-common-sample-bias-persists). Quadratic quadrature errors fall by four on refinement while a common sample bias persists**.

The left plot uses exact [polynomial](polynomial.md) sums; the right adds a common sample bias $\delta=0.002$ to the [composite trapezoidal rule](#composite-trapezoidal-rule). That mathematical model converges to $1/3+\delta$, showing why smaller panels alone do not ensure accuracy for noisy samples. It illustrates [noise sensitivity of a quadrature rule](numerical-integration.md#noise-sensitivity-of-a-quadrature-rule), rather than measured data.

#### Trapezoidal rule fails B-stability

↑ **Parent:** [Trapezoidal rule](#trapezoidal-rule)

The [trapezoidal rule](#trapezoidal-rule) is [A-stable](numerical-analysis.md#a-stability) but is not [B-stable](numerical-analysis.md#b-stability). For the [dissipative vector field](differential-equation.md#dissipative-vector-field) $f(y)=-y^3$ at step size one, its uniquely defined step map $T$ obeys $T+T^3/2=y-y^3/2$. At $y=\sqrt2$, $T=0$ and implicit differentiation gives $T'=-2$, so nearby states expand rather than contract. This is a concrete nonlinear obstruction, rather than merely failure of the sufficient [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) criterion.

## Time-symmetric numerical method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

A one-step numerical method with step map $\Phi_h$ is time symmetric when $\Phi_{-h}=\Phi_h^{-1}$. Its leading local-error power is odd, so every nontrivial consistent time-symmetric method has even order.

## Order of a Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_of_a_Runge-Kutta_method)

The order is the highest power through which the one-step expansion matches the exact Taylor expansion.

### Third-order conditions for an explicit Runge-Kutta method

↑ **Parent:** [Order of a Runge-Kutta method](#order-of-a-runge-kutta-method)

For an explicit [Runge-Kutta method](runge-kutta-method.md) with coefficients $A,b$, put $c=A\mathbf1$ and let $c^2$ mean componentwise squaring. The conditions $b^T\mathbf1=1$, $b^Tc=1/2$, $b^Tc^2=1/3$ and $b^TAc=1/6$ match the exact flow expansion through degree three: the two cubic differentials are $f^{\prime\prime}[f,f]$ and $(f^\prime)^2f$. For sufficiently smooth vector fields these give local error $O(h^4)$ and, under the usual finite-interval [Lipschitz continuity](real-analysis.md#lipschitz-continuity) assumptions, global error $O(h^3)$.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (56)

- [Adaptive Euler step doubling for exponential decay](error-control-for-ode-solvers.md#adaptive-euler-step-doubling-for-exponential-decay)
- [Butcher contractivity theorem](#butcher-contractivity-theorem)
- [Butcher order condition](#butcher-order-condition)
- [Butcher tableau](#butcher-tableau)
- [Classical fourth-order Runge-Kutta method](#classical-fourth-order-runge-kutta-method)
- [Dissipative vector field](differential-equation.md#dissipative-vector-field)
- [Embedded Runge-Kutta pair](error-control-for-ode-solvers.md#embedded-runge-kutta-pair)
- [Energy dissipation of a damped pendulum](simple-pendulum.md#energy-dissipation-of-a-damped-pendulum)
- [Fourth-order conditions for a Runge-Kutta method](#fourth-order-conditions-for-a-runge-kutta-method)
- [Heun's method](#heun-s-method)
- [Maximal-order Runge-Kutta methods are A-stable](#maximal-order-runge-kutta-methods-are-a-stable)
- [Normalized intermediate-axis model](rigid-body-dynamics.md#normalized-intermediate-axis-model)
- [Padé identification of a Radau stability function](#pade-identification-of-a-radau-stability-function)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#38a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#38c/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#39a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#39a/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#4/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#4/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#8d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#18c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#17b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-341.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341.md#section-b/6/solution)
- [Paul trap secular-motion example](atomic-physics.md#paul-trap-secular-motion-example)
- [Runge-Kutta stage](#runge-kutta-stage)
- [Second-order conditions with independent Runge-Kutta abscissae](#second-order-conditions-with-independent-runge-kutta-abscissae)
- [SIR infection peak](mathematical-biology.md#sir-infection-peak)
- [Strong stability preserving Runge-Kutta method](#strong-stability-preserving-runge-kutta-method)
- [Third-order conditions for an explicit Runge-Kutta method](#third-order-conditions-for-an-explicit-runge-kutta-method)
- [Torque-free tumbling](rigid-body-dynamics.md#torque-free-tumbling)
