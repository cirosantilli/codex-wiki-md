# Finite element method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_element_method)

The [finite element method](finite-element-method.md) replaces an infinite-dimensional [weak formulation](partial-differential-equation.md#weak-formulation) by finitely many unknowns attached to a [finite element mesh](#finite-element-mesh). Simple local functions, often [piecewise polynomial functions](polynomial.md#piecewise-polynomial-function), join to form a global approximation. The attraction is that each [finite element](#finite-element) can be integrated separately, while the assembled equations enforce a global balance. A [piecewise-linear hat function](#piecewise-linear-hat-function) only meets its immediate neighbors, so a large problem can have a [sparse matrix](vector-space.md#sparse-matrix) rather than a dense one. Gilbert Strang's MIT lecture develops this connection from the one-dimensional [weak formulation](partial-differential-equation.md#weak-formulation) through local hats to the [stiffness matrix](#stiffness-matrix) and load integrals.[Gilbert Strang, MIT 18.085, Lecture 18: Finite Elements in 1D, transcript pp. 2–8, 2008; accessed 2026-10-11](https://ocw.mit.edu/courses/18-085-computational-science-and-engineering-i-fall-2008/676ba0a00eef45a6cb3823c4da61ee11_18-085F08-L18.pdf)

For the conforming [Galerkin method](partial-differential-equation.md#galerkin-method), let $V$ be a real [Hilbert space](hilbert-space.md), $a$ a bounded [coercive bilinear form](bilinear-form.md#coercive-bilinear-form), and $\ell$ a bounded [linear functional](dual-space.md#linear-functional). Given a [conforming finite element space](#conforming-finite-element-space) $V_h\subset V$, the continuous and discrete problems are

$$
\begin{aligned}
u\in V:&\quad a(u,v)=\ell(v)&&\text{for every }v\in V,\\
u_h\in V_h:&\quad a(u_h,v_h)=\ell(v_h)&&\text{for every }v_h\in V_h.
\end{aligned}
$$

Writing $u_h=\sum_j c_j\phi_j$ in a [basis](vector-space.md#basis) of $V_h$ gives the [linear system](linear-algebra.md#system-of-linear-equations)

$$
Kc=F,\qquad K_{ij}=a(\phi_j,\phi_i),\qquad F_i=\ell(\phi_i).
$$

Here $K$ is the [stiffness matrix](#stiffness-matrix) and $F$ is the vector of loads tested against the [basis](vector-space.md#basis) functions. The [Galerkin method](partial-differential-equation.md#galerkin-method) uses the same trial and test space in this construction. Finite element methods also use the [Petrov-Galerkin method](partial-differential-equation.md#petrov-galerkin-method), with different trial and test spaces; testing against the trial space is therefore a property of this construction, rather than a definition of every [finite element method](finite-element-method.md).

The [finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation) below gives every entry explicitly. Refining the [finite element mesh](#finite-element-mesh) then improves the approximation by adding local degrees of freedom. For a symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form), [Galerkin orthogonality](#galerkin-orthogonality) makes the discrete solution the best approximation in the [energy norm](#energy-norm); the geometry of [orthogonal projection](hilbert-space.md#orthogonal-projection) explains why this local construction yields a globally meaningful answer.

**Table of contents**

- [Finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation)
- [Semidiscrete finite element heat equation](#semidiscrete-finite-element-heat-equation)
  - [Forward Euler limit for a consistent hat mass matrix](#forward-euler-limit-for-a-consistent-hat-mass-matrix)
- [Finite element](#finite-element)
- [Conforming finite element space](#conforming-finite-element-space)
- [Finite element mesh](#finite-element-mesh)
  - [Shape-regular mesh](#shape-regular-mesh)
- [Finite element interpolation estimate](#finite-element-interpolation-estimate)
- [Mass matrix](#mass-matrix)
  - [Mass eigenstate](#mass-eigenstate)
  - [Affine-weighted hat mass matrix](#affine-weighted-hat-mass-matrix)
- [Stiffness matrix](#stiffness-matrix)
  - [Reaction-diffusion finite element matrix](#reaction-diffusion-finite-element-matrix)
- [Energy conservation for semidiscrete Galerkin advection](#energy-conservation-for-semidiscrete-galerkin-advection)
- [Cubic Hermite finite element](#cubic-hermite-finite-element)
- [Rayleigh-Ritz method](#rayleigh-ritz-method)
  - [Trial function](#trial-function)
  - [Affine-parameter Sturm-Liouville eigenvalue bound](#affine-parameter-sturm-liouville-eigenvalue-bound)
  - [Exponential-polynomial trial space for a mixed Sturm-Liouville problem](#exponential-polynomial-trial-space-for-a-mixed-sturm-liouville-problem)
  - [Ritz-Galerkin equivalence for a symmetric coercive form](#ritz-galerkin-equivalence-for-a-symmetric-coercive-form)
    - [Symmetry and coercivity in quadratic energy minimization](#symmetry-and-coercivity-in-quadratic-energy-minimization)
  - [Energy norm](#energy-norm)
- [Galerkin orthogonality](#galerkin-orthogonality)
  - [Céa's lemma](#cea-s-lemma)
    - [Aubin–Nitsche duality argument](#aubin-nitsche-duality-argument)
- [Piecewise-linear hat function](#piecewise-linear-hat-function)

## Finite element solution of the one-dimensional Poisson equation

↑ **Parent:** [Finite element method](finite-element-method.md)

Consider the [Poisson equation](partial-differential-equation.md#poisson-s-equation) on an [interval](real-analysis.md#interval-mathematics) with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition):

$$
-u''(x)=1\quad(0<x<1),\qquad u(0)=u(1)=0.
$$

Two [integrations](integral.md) and the endpoint conditions give the exact solution $u(x)=x(1-x)/2$. To approximate it, multiply by a [test function](distribution-theory.md#test-function) $v$ that vanishes at both endpoints. [Integration by parts](calculus.md#integration-by-parts) gives

$$
\int_0^1(-u'')v\,dx
=\bigl[-u'v\bigr]_0^1+\int_0^1u'v'\,dx
=\int_0^1v\,dx.
$$

The boundary term is zero. Thus the [weak formulation](partial-differential-equation.md#weak-formulation) is to find $u\in V=H_0^1(0,1)$ such that

$$
a(u,v):=\int_0^1u'v'\,dx=\ell(v):=\int_0^1v\,dx\qquad(v\in V).
$$

The [zero-trace Sobolev space](sobolev-space.md#zero-trace-sobolev-space) $H_0^1(0,1)$ consists of square-integrable functions with square-integrable [weak derivatives](distribution-theory.md#weak-derivative) and zero endpoint values in their continuous representatives; it does not require a classical second derivative. This is why continuous [piecewise linear functions](function.md#piecewise-linear-function) are admissible despite corners. The [Poincaré inequality](sobolev-space.md#poincare-inequality) makes $a$ a [coercive bilinear form](bilinear-form.md#coercive-bilinear-form) on $V$. Strang derives this one-dimensional [weak formulation](partial-differential-equation.md#weak-formulation), the [piecewise-linear hat functions](#piecewise-linear-hat-function), and their load and derivative-product integrals in the cited lecture; its endpoint example uses a free left endpoint, while both endpoints here are fixed.[Strang, MIT 18.085, Lecture 18, transcript pp. 2–8: weak form, hat basis, and assembly](https://ocw.mit.edu/courses/18-085-computational-science-and-engineering-i-fall-2008/676ba0a00eef45a6cb3823c4da61ee11_18-085F08-L18.pdf)

Take the uniform [finite element mesh](#finite-element-mesh) $x_j=jh$, $j=0,\ldots,n$, with $h=1/n$. The continuous $P_1$ trial space is

$$
V_h=\{v_h\in C([0,1]):v_h(0)=v_h(1)=0,\quad v_h|_{[x_j,x_{j+1}]}\text{ is affine for every }j\}.
$$

Here $P_1$ means [polynomials](polynomial.md) of degree at most one on each [interval](real-analysis.md#interval-mathematics). This is a [conforming finite element space](#conforming-finite-element-space) in $V$, with $n-1$ interior [piecewise-linear hat functions](#piecewise-linear-hat-function) $\phi_i$ as a [basis](vector-space.md#basis). Their endpoint values enforce the [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) automatically. Set $u_h=\sum_{i=1}^{n-1}c_i\phi_i$ and test the [weak formulation](partial-differential-equation.md#weak-formulation) against each $\phi_i$:

$$
K_{ij}=\int_0^1\phi_j'\phi_i'\,dx,\qquad
F_i=\int_0^1\phi_i\,dx=h,\qquad Kc=F.
$$

Each interior hat has two slopes $1/h$ and $-1/h$, each over a length $h$. Its squared derivative therefore integrates to $2/h$. Adjacent hats have opposite slopes on their one shared [interval](real-analysis.md#interval-mathematics), giving $-1/h$. All other derivative products vanish. The [stiffness matrix](#stiffness-matrix) is the [tridiagonal matrix](vector-space.md#tridiagonal-matrix)

$$
K_{ii}=\frac2h,\qquad K_{i,i+1}=K_{i+1,i}=-\frac1h,\qquad K_{ij}=0\quad(|i-j|>1).
$$

The load $F_i=h$ is the area of a triangle of base $2h$ and height one, including hats next to the boundary. Boundary hats are omitted because the boundary values are prescribed. The [piecewise-linear hat function](#piecewise-linear-hat-function) article explains how the same entries arise by adding local two-node contributions.

With four [mesh](#finite-element-mesh) intervals, $h=1/4$, there are three unknowns:

$$
K=\begin{pmatrix}8&-4&0\\-4&8&-4\\0&-4&8\end{pmatrix},\qquad
F=\begin{pmatrix}1/4\\1/4\\1/4\end{pmatrix},\qquad
c=\begin{pmatrix}3/32\\1/8\\3/32\end{pmatrix}.
$$

For example, the first row gives $8(3/32)-4(1/8)=1/4$ and the middle gives $-4(3/32)+8(1/8)-4(3/32)=1/4$. The [coefficients](vector-space.md#coefficient) are the nodal values $u_h(x_i)=c_i$. At $x=3/8$, [linear interpolation](function.md#linear-interpolation) gives $u_h(3/8)=7/64=0.109375$, whereas $u(3/8)=15/128=0.1171875$: exactness at the nodes still leaves a visible error between them.

In this model the [Galerkin method](partial-differential-equation.md#galerkin-method) solution equals the nodal approximation $I_hu$ obtained by [linear interpolation](function.md#linear-interpolation) on any [finite element mesh](#finite-element-mesh). Indeed, on each [interval](real-analysis.md#interval-mathematics) $[a,b]$, $(I_hu)'$ is the average of $u'$ and $v_h'$ is constant. Therefore $\int_a^b(u'-(I_hu)')v_h'\,dx=0$. Summing proves [Galerkin orthogonality](#galerkin-orthogonality) for $I_hu$, and uniqueness gives $u_h=I_hu$. This argument relies on the constant diffusion coefficient, conformity and exact integration; nodal exactness is not a general promise for [finite element methods](finite-element-method.md) with other operators or integration rules.

On a uniform [mesh](#finite-element-mesh), direct subtraction of the chord from the [parabola](euclidean-geometry.md#parabola) gives, on every element $[a,b]$ of length $h$,

$$
e(x):=u(x)-u_h(x)=\frac{(x-a)(b-x)}2,\qquad
e'(x)=\frac{a+b}2-x.
$$

The largest value error is at an element midpoint. Its size and the [energy norm](#energy-norm) error are exactly

$$
\|e\|_{\infty}=\frac{h^2}{8},\qquad
\|e\|_a^2=\int_0^1|e'|^2\,dx
=n\int_{-h/2}^{h/2}t^2\,dt=\frac{h^2}{12},\qquad
\|e\|_a=\frac{h}{\sqrt{12}}.
$$

Thus $h=1/4$ gives $\|e\|_\infty=1/128=0.0078125$ and $\|e\|_a=1/(4\sqrt{12})\approx0.0721688$. With eight elements, $h=1/8$, these become $1/512=0.001953125$ and $1/(8\sqrt{12})\approx0.0360844$. Halving the [mesh](#finite-element-mesh) spacing quarters the maximum value error but only halves the [energy norm](#energy-norm) error: values and slopes converge at different rates. The figure shows the small value error at its own scale, where the four-to-one reduction becomes clear.

<a id="image-exact-poisson-parabola-and-continuous-piecewise-linear-finite-element-solutions-on-four-and-eight-intervals-with-midpoint-errors-shown-separately"></a>
![](finite-element-poisson-refinement.png)

**[Figure 1](#image-exact-poisson-parabola-and-continuous-piecewise-linear-finite-element-solutions-on-four-and-eight-intervals-with-midpoint-errors-shown-separately). Exact Poisson parabola and continuous piecewise-linear finite element solutions on four and eight intervals, with midpoint errors shown separately**.

## Semidiscrete finite element heat equation

↑ **Parent:** [Finite element method](finite-element-method.md)

The spatial [Galerkin method](partial-differential-equation.md#galerkin-method) for the [heat equation](diffusion-equation.md#heat-equation) gives a [mass matrix](#mass-matrix) $M$ and a diffusion [stiffness matrix](#stiffness-matrix) $S$. With zero forcing, $\frac{d}{dt}(c^TMc)=-2c^TSc\leq0$. The [quadratic form](quadratic-form.md) $c^TMc$ is the squared [L2 norm](real-analysis.md#l2-norm) of the represented finite-element function, proving an energy contraction. For nonzero forcing, the corresponding identity has the additional term $2c^TF$, which can be estimated using the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

### Forward Euler limit for a consistent hat mass matrix

↑ **Parent:** [Semidiscrete finite element heat equation](#semidiscrete-finite-element-heat-equation)

For a uniform piecewise-linear Galerkin heat discretization, the consistent [mass matrix](#mass-matrix) is $M=(h/6)\operatorname{tridiag}(1,4,1)$ and the [stiffness matrix](#stiffness-matrix) is $K=h^{-1}\operatorname{tridiag}(-1,2,-1)$. The generalized [eigenvalues](linear-operator-theory.md#eigenvalue) are $6(1-\cos\theta)/[h^2(2+\cos\theta)]$. Applying [forward Euler method](numerical-analysis.md#euler-method) requires $k\lambda\leq2$, giving the displayed uniform bound for $\mu=k/h^2$. For $J$ intervals with Dirichlet endpoints the exact finite-grid upper bound is $(2-\cos(\pi/J))/[3(1+\cos(\pi/J))]$, which approaches $1/6$. Replacing the consistent [mass matrix](#mass-matrix) by a lumped one changes the [stability](numerical-analysis.md#stability-of-a-numerical-method) restriction.

## Finite element

↑ **Parent:** [Finite element method](finite-element-method.md)

A finite element specifies a reference region, a finite-dimensional space of local trial functions, and degrees of freedom that uniquely determine each such function. Assembling compatible copies over a [finite element mesh](#finite-element-mesh) gives a global trial space. For a one-dimensional linear element, the region is an interval, the functions are [affine functions](vector-space.md#affine-function), and the degrees of freedom are the endpoint values.

## Conforming finite element space

↑ **Parent:** [Finite element method](finite-element-method.md)

A conforming finite element space is a finite-dimensional [vector subspace](vector-space.md#vector-subspace) of the solution's variational space $V$. For a second-order problem with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), continuous piecewise-polynomial functions vanishing on the boundary form such a subspace of the [zero-boundary Sobolev space](sobolev-space.md#zero-boundary-sobolev-space) $H_0^1(\Omega)$. Conformity allows exact [Galerkin orthogonality](#galerkin-orthogonality) and the [Céa lemma](#cea-s-lemma).

## Finite element mesh

↑ **Parent:** [Finite element method](finite-element-method.md)

A [finite element mesh](#finite-element-mesh) partitions a domain into simple regions called elements, such as [intervals](real-analysis.md#interval-mathematics), [triangles](euclidean-geometry.md#triangle) or [tetrahedra](euclidean-geometry.md#tetrahedron). In a conforming partition, distinct element interiors are disjoint, their closures cover the domain closure, and any nonempty intersection is a common face, edge or vertex of both elements. Chen's author notes give this compatibility condition for simplicial [meshes](#finite-element-mesh).[Long Chen, Introduction to Finite Element Methods, §2.1, pp. 3–4; updated January 17, 2024](https://webapps.math.uci.edu/~chenlong/226/Ch2FEM.pdf) Local [piecewise polynomial functions](polynomial.md#piecewise-polynomial-function) and local [integrals](integral.md) are defined on these regions; compatible degrees of freedom join them into a global [conforming finite element space](#conforming-finite-element-space). The assembled [stiffness matrix](#stiffness-matrix) and [mass matrix](#mass-matrix) then inherit the local overlap pattern.

For the [finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation), a [mesh](#finite-element-mesh) is simply an ordered list

$$
0=x_0<x_1<\cdots<x_n=1,\qquad
\mathcal T_h=\{[x_j,x_{j+1}]:0\leq j<n\},\qquad
h=\max_{0\leq j<n}(x_{j+1}-x_j).
$$

Nodes are the endpoints; elements are the intervening [intervals](real-analysis.md#interval-mathematics). Four equal elements have five nodes but only three unknown nodal values after imposing the zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). A nonuniform partition such as $0,1/8,1/4,1/2,1$ has element lengths $1/8,1/8,1/4,1/2$ and $h=1/2$, so counting elements alone does not measure the largest unresolved scale.

Refining a [finite element mesh](#finite-element-mesh) replaces some or all elements by smaller ones. For continuous [piecewise linear functions](function.md#piecewise-linear-function) in one dimension, retaining all old nodes gives nested [conforming finite element spaces](#conforming-finite-element-space) $V_h\subset V_{h/2}$ when every [interval](real-analysis.md#interval-mathematics) is bisected. The old approximation remains available, and the new interior nodes allow additional changes of slope. With a symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form) and exact integration, best approximation from [Galerkin orthogonality](#galerkin-orthogonality) means that the [energy norm](#energy-norm) error cannot increase under such nested refinement.

For the [finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation), uniform refinement from four to eight elements increases the unknown count from three to seven. The exact formulas give maximum errors $0.0078125$ and $0.001953125$, and [energy norm](#energy-norm) errors approximately $0.0721688$ and $0.0360844$. Refinement near a region of strong curvature can spend unknowns where the [linear interpolation](function.md#linear-interpolation) error matters most; convergence in a general problem still needs approximation and regularity assumptions such as those in the [finite element interpolation estimate](#finite-element-interpolation-estimate).

### Shape-regular mesh

↑ **Parent:** [Finite element mesh](#finite-element-mesh)

A family of simplicial meshes is shape-regular when the ratio of each element's diameter to its inscribed-ball radius stays uniformly bounded. This excludes degenerating shapes and makes [finite element interpolation estimates](#finite-element-interpolation-estimate) uniform in the mesh size. The element sizes may still vary substantially across the domain.

## Finite element interpolation estimate

↑ **Parent:** [Finite element method](finite-element-method.md)

On a [shape-regular mesh](#shape-regular-mesh) in dimensions at most three, nodal piecewise-linear interpolation of $u\in H^2(\Omega)$ satisfies

$$
\|u-I_hu\|_{L^2(\Omega)}+h\|u-I_hu\|_{H^1(\Omega)}
\leq Ch^2\|u\|_{H^2(\Omega)},
$$

where $h$ is the largest element diameter and $C$ is independent of $h$. For homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), $I_hu$ belongs to the [conforming finite element space](#conforming-finite-element-space). Scaling each element to a reference element gives the estimate; [shape regularity](#shape-regular-mesh) bounds the scaling constants, while subtraction of an [affine function](vector-space.md#affine-function) leaves an error controlled by the second derivatives.

## Mass matrix

↑ **Parent:** [Finite element method](finite-element-method.md)

The mass matrix is the [Gram matrix](inner-product.md#gram-matrix) of a [finite element](#finite-element) basis in the [L2 inner product](measure-theory.md#l2-inner-product). Its coefficient [quadratic form](quadratic-form.md) is the squared [L2 norm](real-analysis.md#l2-norm) of the represented trial function, so it is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) for a linearly independent basis.

### Mass eigenstate

↑ **Parent:** [Mass matrix](#mass-matrix)

A [mass eigenstate](#mass-eigenstate) diagonalizes the Hermitian [mass](classical-mechanics.md#mass) operator or [mass matrix](#mass-matrix) and has a definite [mass](classical-mechanics.md#mass). In a flavor basis with off-diagonal [mass](classical-mechanics.md#mass) terms, it is a linear combination of flavor states. For unstable particles, decay propagation instead involves an effective complex matrix; its [eigenvectors](linear-operator-theory.md#eigenvector) need not inherit the orthogonality of a Hermitian [mass](classical-mechanics.md#mass) problem.

### Affine-weighted hat mass matrix

↑ **Parent:** [Mass matrix](#mass-matrix)

On a one-dimensional uniform [finite element mesh](#finite-element-mesh) of spacing $h$, let $w$ be an [affine function](vector-space.md#affine-function) and $\phi_i$ the interior [piecewise-linear hat functions](#piecewise-linear-hat-function). The weighted [mass matrix](#mass-matrix) has entries

$$
W_{ii}=\frac{2h}{3}w(x_i),\qquad
W_{i,i+1}=W_{i+1,i}=\frac h{12}\bigl(w(x_i)+w(x_{i+1})\bigr),
$$

and zero entries for nonadjacent indices. The diagonal product $\phi_i^2$ is symmetric about $x_i$ and integrates to $2h/3$; the neighbouring product is symmetric about $(x_i+x_{i+1})/2$ and integrates to $h/6$. The odd part of an [affine function](vector-space.md#affine-function) integrates to zero around each centre, giving the formulas. This evaluates a variable reaction term exactly without substituting a constant coefficient or a quadrature approximation.

## Stiffness matrix

↑ **Parent:** [Finite element method](finite-element-method.md)

The stiffness matrix represents a variational [bilinear form](bilinear-form.md) $a$ in a [finite element](#finite-element) basis. A symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form) gives a [positive-definite matrix](quadratic-form.md#positive-definite-matrix). Local support of the [piecewise-linear hat functions](#piecewise-linear-hat-function) produces a sparse [matrix](vector-space.md#matrix), allowing efficient numerical solution.

### Reaction-diffusion finite element matrix

↑ **Parent:** [Stiffness matrix](#stiffness-matrix)

For $-u''+u=f$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the conforming [piecewise-linear hat functions](#piecewise-linear-hat-function) on a uniform grid give a diffusion [stiffness matrix](#stiffness-matrix) $S$ and a [mass matrix](#mass-matrix) $M$. Their nonzero entries are $S_{ii}=2/h$, $S_{i,i+1}=-1/h$, $M_{ii}=2h/3$, and $M_{i,i+1}=h/6$, with symmetric counterparts. The sum is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) because its coefficient [quadratic form](quadratic-form.md) is $\int((u_h')^2+u_h^2)$. For forcing $f(x)=x$, the load at $x_i$ is $hx_i$.

## Energy conservation for semidiscrete Galerkin advection

↑ **Parent:** [Finite element method](finite-element-method.md)

For periodic $u_t=u_x$, the conforming [Galerkin method](partial-differential-equation.md#galerkin-method) has $M\dot U=CU$, with [mass matrix](#mass-matrix) $M_{ij}=\int\phi_i\phi_j$ and $C_{ij}=\int\phi_i\phi_j'$. [Integration by parts](calculus.md#integration-by-parts) and periodicity give $C^T=-C$. Therefore

$$
\frac{d}{dt}(U^TMU)=2U^TCU=0.
$$

The conserved quantity is the squared [L2 norm](real-analysis.md#l2-norm) of the [finite element](#finite-element) function. On a uniform one-dimensional mesh of spacing $h$, the [piecewise-linear hat functions](#piecewise-linear-hat-function) give $M_{ii}=2h/3$, $M_{i,i\pm1}=h/6$, $C_{i,i+1}=1/2$ and $C_{i,i-1}=-1/2$.

## Cubic Hermite finite element

↑ **Parent:** [Finite element method](finite-element-method.md)

A cubic Hermite finite element is piecewise cubic and joins with continuous first derivative. It is therefore conforming for fourth-order variational problems whose energy space lies in $H^2$.

## Rayleigh-Ritz method

↑ **Parent:** [Finite element method](finite-element-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh–Ritz_method)

The Ritz method minimizes a quadratic energy over a finite-dimensional trial space. For basis functions $\phi_j$ and bilinear form $a$, its linear system is $Ka=F$ with $K_{jk}=a(\phi_k,\phi_j)$ and $F_j=\langle f,\phi_j\rangle$.

### Trial function

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

A trial function is a chosen candidate used to approximate a solution or evaluate a [variational principle](calculus-of-variations.md#variational-principle). For an [eigenvalue](linear-operator-theory.md#eigenvalue) upper bound from a [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient), it must be nonzero, have finite numerator and denominator, and lie in the appropriate variational domain. In a [Dirichlet problem](analysis.md#dirichlet-problem) it satisfies the fixed endpoint values. Natural boundary conditions need not always be imposed on a trial in the quadratic-form domain, but a candidate violating an essential [boundary condition](differential-equation.md#boundary-condition) does not give the stated bound.

### Affine-parameter Sturm-Liouville eigenvalue bound

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

For a self-adjoint [Sturm-Liouville operator](sturm-liouville-theory.md#sturm-liouville-operator) $L_\epsilon=L_0+\epsilon L_1$ with common boundary conditions and an $L^2$-normalized lowest [eigenfunction](linear-operator-theory.md#eigenfunction) $U_0$ of $L_0$, evaluating the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) on $U_0$ gives the displayed upper bound. More generally the lowest eigenvalue is the infimum of affine functions of $\epsilon$, so it is concave in that parameter. The trial state must satisfy the boundary requirements of the variational domain; changing the operator without changing the trial function's normalization can still be legitimate when the weight is fixed.

### Exponential-polynomial trial space for a mixed Sturm-Liouville problem

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

For $-(p y')'=\lambda w y$ on $[0,1]$ with $p=(1+x)e^{2x}$, $w=e^{2x}$, $y(0)=0$ and $y'(1)=0$, the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is $\int p y'^2/\int w y^2$. The trial $y_1=xe^{-x}$ gives numerator $5/12$ and denominator $1/3$, hence $0<\lambda_{\min}\leq5/4$. Every displayed $y_n$ obeys the same mixed [boundary conditions](differential-equation.md#boundary-condition); so does $\sin[(m+1/2)\pi x]$. Adding any of these to the trial space cannot worsen the optimized upper bound. Matrix elements $A_{ij}=\int p y_i'y_j'$ and $M_{ij}=\int w y_iy_j$ give a finite-dimensional [generalized eigenvalue problem](linear-operator-theory.md#generalized-eigenvalue-problem) $Av=\lambda Mv$. The case $n=1$ repeats the original trial and adds no variational freedom.

### Ritz-Galerkin equivalence for a symmetric coercive form

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

For a bounded symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form) on a Hilbert space, a solution of $a(u,w)=\ell(w)$ minimizes $J(v)=a(v,v)/2-\ell(v)$. The displayed identity proves strict minimality and uniqueness. Restricting to a [conforming finite element space](#conforming-finite-element-space) makes the discrete [Ritz method](#rayleigh-ritz-method) equivalent to the [Galerkin method](partial-differential-equation.md#galerkin-method). [Galerkin orthogonality](#galerkin-orthogonality) gives exact best approximation in the [energy norm](#energy-norm); the [Céa lemma](#cea-s-lemma) translates it into a reference-norm estimate.

#### Symmetry and coercivity in quadratic energy minimization

↑ **Parent:** [Ritz-Galerkin equivalence for a symmetric coercive form](#ritz-galerkin-equivalence-for-a-symmetric-coercive-form)

A continuous symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form) $a$ on a real [Hilbert space](hilbert-space.md) and a continuous [linear functional](dual-space.md#linear-functional) $\ell$ give a unique minimum of $I$. The parallelogram identity makes any minimizing sequence Cauchy in the energy norm; coercivity and completeness give its limit. Differentiation gives $a(u,w)=\ell(w)$, and $I(v)-I(u)=a(v-u,v-u)$ proves uniqueness. A nonsymmetric operator instead differentiates to its symmetric part. Mere pointwise positivity without a lower bound in the chosen norm need not yield a minimizing vector.

### Energy norm

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

A symmetric coercive bilinear form $a$ defines the energy norm $\|v\|_a=\sqrt{a(v,v)}$. In this norm the [Ritz method](#rayleigh-ritz-method) is an orthogonal projection onto its finite-dimensional trial space.

## Galerkin orthogonality

↑ **Parent:** [Finite element method](finite-element-method.md)

Let $V_h\subset V$ be a [conforming finite element space](#conforming-finite-element-space). Suppose the exact solution satisfies $a(u,v)=\ell(v)$ for every $v\in V$ and its [Galerkin method](partial-differential-equation.md#galerkin-method) approximation satisfies $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$, using the same [bilinear form](bilinear-form.md) and [linear functional](dual-space.md#linear-functional). Subtracting the two identities gives [Galerkin orthogonality](#galerkin-orthogonality):

$$
a(u-u_h,v_h)=0\qquad(v_h\in V_h).
$$

This identity itself does not require symmetry. Its interpretation as an [orthogonal projection](hilbert-space.md#orthogonal-projection) in an [energy norm](#energy-norm) does require a bounded symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form): then $a$ is an [inner product](inner-product.md), $e=u-u_h$ is perpendicular to every available discrete correction, and

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2\qquad(v_h\in V_h).
$$

Consequently $u_h$ is the unique closest point in $V_h$ in the [energy norm](#energy-norm). This [Pythagorean theorem](euclidean-geometry.md#pythagorean-theorem) in a function space explains the beauty of the [Galerkin method](partial-differential-equation.md#galerkin-method): integrated local equations compute a global best approximation. The [Céa lemma](#cea-s-lemma) supplies the corresponding estimate in a chosen reference norm.

For the [finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation), $a(w,v)=\int_0^1w'v'\,dx$ and $\|w\|_a=\|w'\|_{L^2(0,1)}$. Testing the error against the $i$th [piecewise-linear hat function](#piecewise-linear-hat-function) on a uniform [mesh](#finite-element-mesh) gives

$$
\frac1h\int_{x_{i-1}}^{x_i}e'\,dx
-\frac1h\int_{x_i}^{x_{i+1}}e'\,dx=0.
$$

In this model $e$ vanishes at every node, so each of these [integrals](integral.md) is individually zero, although $e$ is positive inside every element. [Galerkin orthogonality](#galerkin-orthogonality) controls the derivative-weighted balance; it does not say that the pointwise error vanishes.

The exact identity assumes conformity and exact evaluation of the continuous forms, including any [numerical integration](numerical-integration.md) that is used. If assembly instead uses $a_h$ and $\ell_h$, subtraction gives the consistency defect

$$
a(u-u_h,v_h)=(\ell-\ell_h)(v_h)+(a_h-a)(u_h,v_h).
$$

Thus inexact [numerical integration](numerical-integration.md) need not preserve the projection. In the [Petrov-Galerkin method](partial-differential-equation.md#petrov-galerkin-method) the error is tested against a different test space, and for a nonsymmetric [bilinear form](bilinear-form.md) the displayed identity need not describe perpendicularity in any [energy norm](#energy-norm).

<h3 id="cea-s-lemma">Céa's lemma</h3>

↑ **Parent:** [Galerkin orthogonality](#galerkin-orthogonality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Céa's_lemma)

For a continuous coercive bilinear form with continuity constant $M$ and coercivity constant $\alpha$, a conforming finite-element solution satisfies

$$
\|u-u_h\|_V\leq\frac M\alpha
\inf_{v_h\in V_h}\|u-v_h\|_V.
$$

For a symmetric problem measured in its [energy norm](#energy-norm), the constant is one.

For any $v_h\in V_h$, [Galerkin orthogonality](#galerkin-orthogonality) gives $a(e,e)=a(e,u-v_h)$, where $e=u-u_h$. Coercivity and continuity yield $\alpha\|e\|_V^2\leq M\|e\|_V\|u-v_h\|_V$. Divide by $\|e\|_V$ when it is nonzero and take the infimum. In the symmetric case, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) in the [energy norm](#energy-norm) gives the constant one.

<h4 id="aubin-nitsche-duality-argument">Aubin–Nitsche duality argument</h4>

↑ **Parent:** [Céa's lemma](#cea-s-lemma)

For a symmetric elliptic variational problem with [Galerkin orthogonality](#galerkin-orthogonality), let $e=u-u_h$ and solve the dual problem $a(v,z)=(e,v)_{L^2}$ for every $v\in H_0^1(\Omega)$. If [elliptic regularity](distribution-theory.md#elliptic-regularity) gives $\|z\|_{H^2}\leq C\|e\|_{L^2}$, then a [finite element interpolation estimate](#finite-element-interpolation-estimate) gives

$$
\|e\|_{L^2}^2=a(e,z-I_hz)
\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Thus $\|e\|_{L^2}\leq Ch\|e\|_{H^1}$. Combining this with the [Céa lemma](#cea-s-lemma) and an $O(h)$ [energy norm](#energy-norm) error gives an $O(h^2)$ [L2 norm](real-analysis.md#l2-norm) error. The additional order depends on the dual regularity assumption, which can fail on unsuitable domains.

## Piecewise-linear hat function

↑ **Parent:** [Finite element method](finite-element-method.md)

A [piecewise-linear hat function](#piecewise-linear-hat-function) is a continuous [piecewise linear function](function.md#piecewise-linear-function) that selects one node of a [finite element mesh](#finite-element-mesh): it is one there and zero at every other node. For an interior node $x_i$, its exact formula on a possibly nonuniform [mesh](#finite-element-mesh) is

$$
\phi_i(x)=\begin{cases}
(x-x_{i-1})/(x_i-x_{i-1}),&x_{i-1}\leq x\leq x_i,\\
(x_{i+1}-x)/(x_{i+1}-x_i),&x_i\leq x\leq x_{i+1},\\
0,&\text{otherwise}.
\end{cases}
$$

Its [support of a function](function.md#support) is $[x_{i-1},x_{i+1}]$. It rises on the left [interval](real-analysis.md#interval-mathematics) and falls on the right, producing its hat-shaped graph. The interior [hat functions](#piecewise-linear-hat-function) form a [basis](vector-space.md#basis) of the continuous $P_1$ [conforming finite element space](#conforming-finite-element-space) with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). Chen's author notes define this nodal [basis](vector-space.md#basis) and illustrate it in one and two dimensions.[Chen, Introduction to Finite Element Methods, §3.1, pp. 5–6 and Figure 5: nodal hat basis](https://webapps.math.uci.edu/~chenlong/226/Ch2FEM.pdf) The nodal property $\phi_i(x_j)=\delta_{ij}$ makes the [coefficients](vector-space.md#coefficient) directly readable: if $v_h=\sum_i c_i\phi_i$, then $v_h(x_i)=c_i$. Unlike the global [Lagrange cardinal polynomials](interpolation.md#lagrange-cardinal-polynomial), each of these functions is confined to two neighboring elements.

For example, with $x_j=j/4$, the middle [hat function](#piecewise-linear-hat-function) is $\phi_2(x)=4x-1$ on $[1/4,1/2]$, $3-4x$ on $[1/2,3/4]$, and zero elsewhere. Hence $\phi_2(3/8)=1/2$, while $\phi_1(3/8)=1/2$ and $\phi_3(3/8)=0$. The [finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation) therefore has $u_h(3/8)=(3/32)/2+(1/8)/2=7/64$.

Local assembly makes this locality computational. On an element $[a,b]$ of length $d=b-a$, the two local [basis](vector-space.md#basis) functions are $N_L=(b-x)/d$ and $N_R=(x-a)/d$. For the [Poisson equation](partial-differential-equation.md#poisson-s-equation) with unit forcing, their local [stiffness matrix](#stiffness-matrix) and load vector are

$$
K^{(e)}=\frac1d\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\qquad
F^{(e)}=\frac d2\begin{pmatrix}1\\1\end{pmatrix}.
$$

Add these four matrix entries and two loads to the rows and columns belonging to the element's endpoints, then impose the prescribed boundary values. An interior node receives contributions from its two neighboring elements. Writing $d_L=x_i-x_{i-1}$ and $d_R=x_{i+1}-x_i$ gives

$$
K_{ii}=\frac1{d_L}+\frac1{d_R},\qquad
K_{i,i-1}=-\frac1{d_L},\qquad K_{i,i+1}=-\frac1{d_R},\qquad
F_i=\frac{d_L+d_R}{2},
$$

with off-diagonal entries included only for interior neighbors. On a uniform [mesh](#finite-element-mesh) these reduce to $2/h$, $-1/h$ and $h$. Nonadjacent [hat functions](#piecewise-linear-hat-function) have no derivative overlap of positive length, so all distant entries vanish. This produces a [sparse matrix](vector-space.md#sparse-matrix) with only three diagonals: the global coupling is built entirely from local two-node interactions.

<a id="image-three-interior-hat-functions-on-a-four-interval-mesh-with-local-stiffness-and-load-contributions-assembled-into-the-three-unknown-poisson-system"></a>
![](finite-element-hat-assembly.png)

**[Figure 2](#image-three-interior-hat-functions-on-a-four-interval-mesh-with-local-stiffness-and-load-contributions-assembled-into-the-three-unknown-poisson-system). Three interior hat functions on a four-interval mesh, with local stiffness and load contributions assembled into the three-unknown Poisson system**.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (8)

- [Finite element method](finite-element-method.md)
- [Finite element solution of the one-dimensional Poisson equation](#finite-element-solution-of-the-one-dimensional-poisson-equation)
- [Multigrid method](multigrid-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341.md#6/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2.md#section-b/b7/solution)
