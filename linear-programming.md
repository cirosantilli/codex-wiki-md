# Linear programming

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_programming)

Linear programming optimizes a [linear function](vector-space.md#linear-function) subject to finitely many linear equalities and inequalities.

**Table of contents**

- [Karmarkar standard form](#karmarkar-standard-form)
- [Surplus variable](#surplus-variable)
- [Optimal face of a linear program](#optimal-face-of-a-linear-program)
- [Rational feasibility certificate for integer inequalities](#rational-feasibility-certificate-for-integer-inequalities)
- [Ellipsoid method](#ellipsoid-method)
  - [Feasible-point box bound for a polyhedron with lines](#feasible-point-box-bound-for-a-polyhedron-with-lines)
  - [Full-dimensional relaxation of integer inequalities](#full-dimensional-relaxation-of-integer-inequalities)
  - [Exact linear optimization from a feasibility oracle](#exact-linear-optimization-from-a-feasibility-oracle)
  - [Central-cut ellipsoid volume bound](#central-cut-ellipsoid-volume-bound)
- [Maximum feasible subsystem](#maximum-feasible-subsystem)
- [Linear polyhedron](#linear-polyhedron)
  - [Full-dimensional linear polyhedron](#full-dimensional-linear-polyhedron)
  - [Active constraint](#active-constraint)
    - [Integer-matrix vertex coordinate bound](#integer-matrix-vertex-coordinate-bound)
  - [Strict separation of disjoint linear polyhedra](#strict-separation-of-disjoint-linear-polyhedra)
- [Slack variable](#slack-variable)
- [Bernstein linear programming hierarchy for polynomial minimization](#bernstein-linear-programming-hierarchy-for-polynomial-minimization)
- [Basic feasible solution](#basic-feasible-solution)
  - [Degeneracy in linear programming](#degeneracy-in-linear-programming)
  - [Basic solution](#basic-solution)
  - [Fundamental theorem of linear programming](#fundamental-theorem-of-linear-programming)
- [Linear-fractional programming](#linear-fractional-programming)
  - [Charnes-Cooper transformation](#charnes-cooper-transformation)
- [Linear programming duality](#linear-programming-duality)
  - [Dual feasibility](#dual-feasibility)
  - [Dual of a maximum of affine functions](#dual-of-a-maximum-of-affine-functions)
  - [Lagrangian dual problem](#lagrangian-dual-problem)
    - [Lagrange dual function](#lagrange-dual-function)
    - [Lagrangian relaxation](#lagrangian-relaxation)
      - [Lagrangian knapsack bound](#lagrangian-knapsack-bound)
  - [Dual linear program](#dual-linear-program)
    - [Dual variable](#dual-variable)
  - [Dual of a minimization linear program in inequality form](#dual-of-a-minimization-linear-program-in-inequality-form)
  - [Weak duality](#weak-duality)
    - [Linear programming optimality certificate](#linear-programming-optimality-certificate)
    - [Strong duality](#strong-duality)
      - [Convex perturbation function](#convex-perturbation-function)
        - [Convex perturbation duality](#convex-perturbation-duality)
          - [Sensitivity analysis in convex perturbation duality](#sensitivity-analysis-in-convex-perturbation-duality)
      - [Slater's condition](#slater-s-condition)
      - [Exact maximum-violation penalty](#exact-maximum-violation-penalty)
      - [Dual attainment](#dual-attainment)
    - [Duality gap](#duality-gap)
  - [Complementary slackness](#complementary-slackness)
  - [Transportation problem](#transportation-problem)
    - [Production costs in a transportation problem](#production-costs-in-a-transportation-problem)
    - [Transportation dual potentials](#transportation-dual-potentials)
      - [Transportation dual certificate with capacity inequalities](#transportation-dual-certificate-with-capacity-inequalities)
    - [Assignment problem](#assignment-problem)
      - [Assignment lower bound from independent task minima](#assignment-lower-bound-from-independent-task-minima)
      - [Hungarian algorithm](#hungarian-algorithm)
      - [Assignment dual potentials](#assignment-dual-potentials)
    - [Transportation polytope](#transportation-polytope)
      - [Transportation spanning tree](#transportation-spanning-tree)
    - [Transportation simplex algorithm](#transportation-simplex-algorithm)
      - [Northwest corner method](#northwest-corner-method)
      - [Reduced cost](#reduced-cost)
      - [Cycle pivot](#cycle-pivot)
    - [Integrality of the transportation problem](#integrality-of-the-transportation-problem)
      - [Totally unimodular matrix](#totally-unimodular-matrix)
- [Simplex method](#simplex-method)
  - [Simplex optimality criterion](#simplex-optimality-criterion)
  - [Greatest improvement pivot rule](#greatest-improvement-pivot-rule)
  - [Dantzig pivot rule](#dantzig-pivot-rule)
  - [Klee-Minty cube](#klee-minty-cube)
  - [Simplex tableau](#simplex-tableau)
    - [Reconstructing a linear program from a final simplex tableau](#reconstructing-a-linear-program-from-a-final-simplex-tableau)
    - [Simplex objective update for a priced slack variable](#simplex-objective-update-for-a-priced-slack-variable)
  - [Bland pivoting rule](#bland-pivoting-rule)
  - [Two-phase simplex](#two-phase-simplex)
  - [Simplex ratio test](#simplex-ratio-test)
  - [Simplex basis](#simplex-basis)
    - [Nonbasic variable](#nonbasic-variable)
    - [Basic variable](#basic-variable)
    - [Linear programming sensitivity within a fixed optimal basis](#linear-programming-sensitivity-within-a-fixed-optimal-basis)
      - [Strictly positive dual certificate and right-hand-side sensitivity](#strictly-positive-dual-certificate-and-right-hand-side-sensitivity)
  - [Simplex paths on a cube with one truncated corner](#simplex-paths-on-a-cube-with-one-truncated-corner)

## Karmarkar standard form

↑ **Parent:** [Linear programming](linear-programming.md)

This form of [linear programming](linear-programming.md) additionally has the uniform [vector](vector-space.md#vector) as a strictly positive [feasible point](mathematical-optimization.md#feasible-point) and known optimum zero. A [homogeneous self-dual embedding of a linear program](convex-optimization.md#homogeneous-self-dual-embedding-of-a-linear-program), followed by elimination of unrestricted [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier) and normalization by the sum of nonnegative coordinates, yields this form without presupposing feasibility of the original program. The known start and optimum support projective [interior-point methods](convex-optimization.md#interior-point-method). Polynomial bit-complexity statements additionally require finite rational input encoding; bounded arbitrary real coefficients alone do not provide it.

## Surplus variable

↑ **Parent:** [Linear programming](linear-programming.md)

A surplus variable converts a lower-bound inequality $a^Tx\ge b$ into $a^Tx-z=b$, with $z\ge0$. This is the lower-bound counterpart of a [slack variable](#slack-variable). When the original coefficients, right-hand side and decision variables are integer, the surplus variable is integer as well; that fact permits it to appear in an all-integer [Gomory fractional cut](mathematical-optimization.md#gomory-fractional-cut) row.

## Optimal face of a linear program

↑ **Parent:** [Linear programming](linear-programming.md)

The set of minimizers of a linear objective on a [linear polyhedron](#linear-polyhedron). It is a face: if a strict convex combination of two feasible points minimizes the objective, both points must also minimize it. Hence an [extreme point](convex-set.md#extreme-point) of an optimal face is an extreme point of the original polyhedron. Successively minimizing further linear objectives restricts to nested faces, whose vertices remain original vertices. This preserves uniform rational denominator bounds in exact feasibility-oracle optimization.

## Rational feasibility certificate for integer inequalities

↑ **Parent:** [Linear programming](linear-programming.md)

A nonempty [linear polyhedron](#linear-polyhedron) with integer inequality coefficients and right sides bounded by $U\geq1$ contains a point $x_i=p_i/q_i$ with the displayed bounds. Intersect with an orthant containing a feasible point. Moving along directions annihilating the active constraints, until another constraint becomes active, produces a vertex: the orthant prevents a whole nontrivial line from remaining feasible. At that vertex, choose $n$ independent active inequalities, including coordinate constraints as necessary. [Cramer's rule](multilinear-algebra.md#cramer-s-rule) and the [Hadamard determinant inequality](multilinear-algebra.md#hadamard-determinant-inequality) bound both determinants by $n^{n/2}U^n\leq(nU)^n$. The resulting rational witness has polynomial binary length and is verifiable in [polynomial time](theoretical-computer-science.md#polynomial-time), proving that integer linear feasibility is in [NP](theoretical-computer-science.md#np-complexity).

## Ellipsoid method

↑ **Parent:** [Linear programming](linear-programming.md)

The [ellipsoid method](#ellipsoid-method) repeatedly asks a [separation oracle](convex-optimization.md#separation-oracle) about the center of a containing ellipsoid and replaces that ellipsoid by a smaller one containing its intersection with a separating half-space. The volume decreases by a dimension-dependent factor at each iteration. For rational polyhedra, the exact feasibility theorem has polynomial bit complexity in the dimension and coefficient encoding bounds when separation is [polynomial time](theoretical-computer-science.md#polynomial-time). It includes lower-dimensional feasible sets through rational precision bounds or suitable relaxations; one must not declare infeasibility just because the original feasible set has zero volume.

### Feasible-point box bound for a polyhedron with lines

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

A nonempty [linear polyhedron](#linear-polyhedron) can have no extreme point. Intersect it with an orthant containing one feasible point, and minimize the sum of the signed coordinates there. The relevant sublevel sets are compact, so the minimum face has an extreme point, which is also extreme in the orthant intersection. The added signed-coordinate rows are integer rows with entries at most one. The [integer-matrix vertex coordinate bound](#integer-matrix-vertex-coordinate-bound) gives $R=n!\max(1,U)^n$. This supplies a bounded feasibility search even when the original polyhedron contains lines.

### Full-dimensional relaxation of integer inequalities

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

For an integer [linear polyhedron](#linear-polyhedron) $P=\{x\in\mathbb R^n:Ax\geq b\}$ with coefficients bounded by $U\geq1$, put $D=[(n+1)U]^{n+1}$ and $0<\varepsilon<1/D$. If $x_0\in P$, every $h$ with $\|h\|_2\leq\varepsilon/(nU)$ satisfies $A_i h\geq-\sqrt n U\|h\|_2\geq-\varepsilon$. Thus $P_\varepsilon$ contains a positive-radius [Euclidean ball](normed-vector-space.md#euclidean-ball) and is a [full-dimensional linear polyhedron](#full-dimensional-linear-polyhedron). If $P$ is empty, the [normalized integer Farkas infeasibility gap](convex-optimization.md#normalized-integer-farkas-infeasibility-gap) gives $\lambda\geq0$, $A^T\lambda=0$, $\mathbf1^T\lambda=1$ and $b^T\lambda\geq1/D$. A point of $P_\varepsilon$ would give $0=\lambda^TAx\geq b^T\lambda-\varepsilon>0$, a contradiction. Consequently this relaxation preserves emptiness and supplies the inner-volume bound needed by the [ellipsoid method](#ellipsoid-method), even when $P$ has empty interior.

### Exact linear optimization from a feasibility oracle

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

A [polynomial-time algorithm](theoretical-computer-science.md#polynomial-time-algorithm) for integer linear feasibility gives exact rational [linear programming](linear-programming.md) optimization. Rational vertex bounds give a polynomial-bit bound on every finite optimal value and its denominator. An objective threshold below that bound detects unboundedness after feasibility is established. Binary search with the additional inequality $c^Tx\leq t$ localizes the finite optimum to an interval containing a unique rational of bounded denominator; [continued fractions](diophantine-approximation.md#continued-fraction) recover it exactly. A feasible optimizer can then be found by successive coordinate minimizations on a bounded optimal face. These produce faces of one fixed rational polytope, so one uniform vertex-denominator bound works throughout, avoiding exponential growth of precision requirements.

### Central-cut ellipsoid volume bound

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

For $n\geq2$, the standard ellipsoid covering a centrally cut half of the unit ball has center $e_1/(n+1)$ and shape matrix $D'=\frac{n^2}{n^2-1}(I-\frac2{n+1}e_1e_1^T)$. Its eigenvalues are $n^2/(n+1)^2$ along $e_1$ and $n^2/(n^2-1)$ in the other directions. Hence its volume ratio is $R=\frac n{n+1}(\frac{n^2}{n^2-1})^{(n-1)/2}$. Using $\log(1-a)<-a$ and $\log(1+b)<b$ gives $\log R<-1/(2(n+1))$. Affine changes of coordinates preserve the volume ratio. The resulting geometric convergence underlies the [ellipsoid method](#ellipsoid-method); exact rational feasibility additionally needs input-dependent size, precision and lower-dimensional feasibility bounds.

## Maximum feasible subsystem

↑ **Parent:** [Linear programming](linear-programming.md)

Given finitely encoded linear inequalities, a [maximum feasible subsystem](#maximum-feasible-subsystem) is a largest collection that can be simultaneously satisfied. Its decision version asks whether some $k$ inequalities admit a common solution. This is [NP-complete](theoretical-computer-science.md#np-completeness), despite [polynomial time](theoretical-computer-science.md#polynomial-time) feasibility testing for each fixed collection. For a graph, use nonnegative variables $x_v$, constraints $x_v\geq1$ for vertices, and $M>|V|$ copies of $x_u+x_v\leq1$ for each edge. A subsystem of size $M|E|+k$ must retain a copy of every edge constraint and at least $k$ vertex constraints; those vertices form an [independent set](graph-theory.md#independent-set-graph-theory). Conversely an [independent set](graph-theory.md#independent-set-graph-theory) of size $k$ supplies such a feasible subsystem by its indicator vector.

## Linear polyhedron

↑ **Parent:** [Linear programming](linear-programming.md)

A linear polyhedron is an intersection of finitely many closed affine half-spaces in finite-dimensional real space. It may be empty, unbounded, or lower-dimensional. This usage differs from a three-dimensional geometric [polyhedron](euclidean-geometry.md#polyhedron). The [strict separation of disjoint linear polyhedra](#strict-separation-of-disjoint-linear-polyhedra) follows from [linear programming duality](#linear-programming-duality).

### Full-dimensional linear polyhedron

↑ **Parent:** [Linear polyhedron](#linear-polyhedron)

A [linear polyhedron](#linear-polyhedron) in $\mathbb R^n$ is full-dimensional when its [affine hull](vector-space.md#affine-hull) is all of $\mathbb R^n$. Equivalently, it contains an open [Euclidean ball](normed-vector-space.md#euclidean-ball). An open [Euclidean ball](normed-vector-space.md#euclidean-ball) spans the ambient space. Conversely, a full-dimensional [convex set](convex-set.md) contains $n+1$ affinely independent points; their [convex hull](convex-set.md#convex-hull) is a simplex with nonempty interior, so the set contains an open [Euclidean ball](normed-vector-space.md#euclidean-ball).

### Active constraint

↑ **Parent:** [Linear polyhedron](#linear-polyhedron)

An inequality constraint which holds with equality at the point under consideration. For $Ax\geq b$, a direction annihilating every active row permits sufficiently small feasible moves of either sign. If the active rows have rank $n$, their common solution is a [basic feasible solution](#basic-feasible-solution); the independent equalities uniquely determine it.

#### Integer-matrix vertex coordinate bound

↑ **Parent:** [Active constraint](#active-constraint)

At an [extreme point](convex-set.md#extreme-point) of $\{x:Ax\ge b\}$, the active rows span the ambient dimension: otherwise a nonzero direction orthogonal to all active rows permits small feasible moves of both signs. Select $n$ independent active rows to form an integer matrix $B$. Its nonzero determinant has absolute value at least one. [Cramer's rule](multilinear-algebra.md#cramer-s-rule) and the determinant expansion bound each coordinate by $n!U^n$, where $U$ bounds the entries of $A$ and $b$. The vector $b$ may be real; only the denominator matrix needs to be integer.

### Strict separation of disjoint linear polyhedra

↑ **Parent:** [Linear polyhedron](#linear-polyhedron)

Nonempty disjoint [linear polyhedra](#linear-polyhedron) $P=\{x:Ax\leq b\}$ and $Q=\{y:Cy\leq d\}$ admit $h$ with a strictly positive separation gap. A phase-I [linear program](linear-programming.md) minimizing common constraint violation has positive attained optimum. Its [Lagrangian dual problem](#lagrangian-dual-problem) gives nonnegative $\lambda,\mu$ with $A^T\lambda+C^T\mu=0$ and $\lambda^Tb+\mu^Td<0$. Then $h=A^T\lambda$ satisfies $h^Tx\leq\lambda^Tb<-\mu^Td\leq h^Ty$. The polyhedral hypothesis matters; arbitrary disjoint closed convex sets need not have a positive separation gap.

## Slack variable

↑ **Parent:** [Linear programming](linear-programming.md)

A slack variable turns an inequality constraint $a^Tx\le b$ into the equality $a^Tx+s=b$ with $s\ge0$. Its value measures the unused amount of the constraint. In the [simplex algorithm](numerical-analysis.md#simplex-algorithm), slack variables often supply the initial [basic feasible solution](#basic-feasible-solution).

## Bernstein linear programming hierarchy for polynomial minimization

↑ **Parent:** [Linear programming](linear-programming.md)

For $f$ of degree $d$ and $n\ge\max(1,d)$, compute its degree-$n$ [Bernstein basis](functional-analysis.md#bernstein-basis) coefficients and solve $\max\lambda$ subject to $\lambda\le \beta_{k,n}$, $0\le k\le n$. This is a linear program with $n+1$ inequalities. The coefficients form a convex-combination enclosure of the polynomial values, so $v_n\le\min f$. [Degree elevation of Bernstein coefficients](functional-analysis.md#degree-elevation-of-bernstein-coefficients) makes the bounds monotone. For every $\epsilon>0$, the polynomial $f-(\min f-\epsilon)$ is strictly positive, so [positive Bernstein coefficients for a strictly positive polynomial](functional-analysis.md#positive-bernstein-coefficients-for-a-strictly-positive-polynomial) gives an eventual feasible bound $\min f-\epsilon$. Hence $v_n$ converges to the true minimum. Earlier indices $n<d$ can use a one-inequality program at any common coefficient-based lower bound, preserving the stated constraint count for every positive index.

## Basic feasible solution

↑ **Parent:** [Linear programming](linear-programming.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Basic_feasible_solution)

For $Ax=b$, $x\geq0$, a feasible vector $x$ is basic when the columns $A_i$ indexed by its positive coordinates are linearly independent. Equivalently, enlarge those columns to a basis, set every nonbasic coordinate to zero, and solve the resulting square system.

### Degeneracy in linear programming

↑ **Parent:** [Basic feasible solution](#basic-feasible-solution)

A [basic feasible solution](#basic-feasible-solution) is degenerate when one or more of its basic variables is zero. A [simplex algorithm](numerical-analysis.md#simplex-algorithm) pivot may then change the basis without moving the feasible point or changing the objective. Assignment networks force many zero-flow basic tree arcs.

### Basic solution

↑ **Parent:** [Basic feasible solution](#basic-feasible-solution)

For a full-row-rank system $Ax=b$ with $m$ rows, choose $m$ linearly independent columns, set all remaining variables to zero, and solve the resulting square system. The resulting vector is a basic solution; it is feasible when it also satisfies the required nonnegativity constraints.

### Fundamental theorem of linear programming

↑ **Parent:** [Basic feasible solution](#basic-feasible-solution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_of_linear_programming)

If a linear program has an optimal solution, it has an optimal [basic feasible solution](#basic-feasible-solution). Choose an optimum with minimal positive support. A dependence among its active columns gives a feasible two-sided perturbation; optimality makes its objective slope zero, and moving until one coordinate vanishes contradicts minimality.

## Linear-fractional programming

↑ **Parent:** [Linear programming](linear-programming.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear-fractional_programming)

Linear-fractional programming optimizes a ratio $c^Tx/d^Tx$ over a polyhedron on which the denominator is positive.

### Charnes-Cooper transformation

↑ **Parent:** [Linear-fractional programming](#linear-fractional-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Charnes-Cooper_transformation)

For $d^Tx>0$, set

$$
y=\frac{x}{d^Tx},
\qquad
t=\frac1{d^Tx}.
$$

Then $d^Ty=1$, and $Ax=b$ becomes $Ay=bt$, turning a linear-fractional program into a linear program with objective $c^Ty$.

## Linear programming duality

↑ **Parent:** [Linear programming](linear-programming.md)

Every linear maximization program has a dual minimization program whose feasible objective values bound the primal values.

### Dual feasibility

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

For minimization with constraints $Ax=b$, $x\geq0$, a dual-feasible vector $y$ obeys $A^Ty\leq c$, so $b^Ty$ is a lower bound on every primal-feasible objective value. For a [simplex dictionary](numerical-analysis.md#simplex-dictionary) with basis matrix $B$, the associated vector is $y^T=c_B^TB^{-1}$. Its basic reduced costs are zero and its nonbasic reduced costs are $c_N^T-c_B^TB^{-1}A_N$. Thus nonnegative [reduced costs](#reduced-cost) are exactly dual feasibility in this minimization convention; basic primal values may still be negative, as in the [dual simplex algorithm](numerical-analysis.md#dual-simplex-algorithm).

### Dual of a maximum of affine functions

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

Minimizing $\max_i(a_i^Tx+b_i)$ over unrestricted $x$ is a [linear program](linear-programming.md) after introducing an [epigraph](calculus-of-variations.md#epigraph) variable $t$ and inequalities $a_i^Tx+b_i\leq t$. Its [optimization Lagrangian](mathematical-optimization.md#optimization-lagrangian) has finite infimum over $x,t$ exactly when the nonnegative multipliers sum to one and their weighted slopes sum to zero. The displayed [Lagrangian dual problem](#lagrangian-dual-problem) maximizes the resulting constant lower bound. It identifies the role of a zero-slope [convex combination](convex-set.md#convex-combination) of the affine functions.

### Lagrangian dual problem

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

For a minimization problem with inequalities $g_i(x)\leq0$, the [Lagrangian](calculus-of-variations.md#lagrangian) is $L(x,\lambda)=f(x)+\sum_i\lambda_i g_i(x)$ with $\lambda_i\geq0$. The Lagrangian dual maximizes the concave dual function $q(\lambda)=\inf_xL(x,\lambda)$.

#### Lagrange dual function

↑ **Parent:** [Lagrangian dual problem](#lagrangian-dual-problem)

The [Lagrange dual function](#lagrange-dual-function) is the infimum of a [Lagrangian](calculus-of-variations.md#lagrangian) over its primal variables. It is concave in the multipliers, even before convexity of the primal problem is assumed. Maximizing it over sign-compatible multipliers gives a lower bound on a minimization problem by [weak duality](#weak-duality); appropriate convex qualifications give [strong duality](#strong-duality).

#### Lagrangian relaxation

↑ **Parent:** [Lagrangian dual problem](#lagrangian-dual-problem)

A Lagrangian relaxation moves selected constraints into the objective with appropriately signed [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier). Maximizing the relaxed objective over a larger easy set gives an upper bound for a constrained maximization problem. Optimizing that bound need not solve the original integer problem.

##### Lagrangian knapsack bound

↑ **Parent:** [Lagrangian relaxation](#lagrangian-relaxation)

For binary [knapsack optimization](mathematical-optimization.md#0-1-knapsack-problem), $U(\lambda)$ is an upper bound for every $\lambda\geq0$. Its minimum is computable from the finitely many profit-to-weight breakpoints and agrees with the [fractional knapsack problem](mathematical-optimization.md#fractional-knapsack-problem) optimum. Zero-weight positive-profit terms are added independently.

### Dual linear program

↑ **Parent:** [Linear programming duality](#linear-programming-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_linear_program)

For a primal maximization problem $Ax\leq b$, $x\geq0$, the dual minimizes $b^Ty$ subject to $A^Ty\geq c$, $y\geq0$.

#### Dual variable

↑ **Parent:** [Dual linear program](#dual-linear-program)

A [dual variable](#dual-variable) is a multiplier associated with a primal constraint in a [dual linear program](#dual-linear-program). In a minimization [linear program](linear-programming.md) with equality constraints $Ax=b$ and nonnegative primal variables, the [Lagrangian](calculus-of-variations.md#lagrangian) $c^Tx+y^T(b-Ax)$ yields the dual objective $b^Ty$ and inequalities $A^Ty\le c$; the equality-constraint multipliers $y$ are unrestricted in sign. For a [transportation problem](#transportation-problem), row and column [dual variables](#dual-variable) give potentials $u_i,v_j$ satisfying $u_i+v_j\le c_{ij}$. [Complementary slackness](#complementary-slackness) makes occupied routes attain equality.

### Dual of a minimization linear program in inequality form

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

The dual pair

$$
\min\{c^Tx:Ax\geq b,\ x\geq0\}
\quad\hbox{and}\quad
\max\{b^Ty:A^Ty\leq c,\ y\geq0\}
$$

satisfies weak duality because $b^Ty\leq y^TAx=x^TA^Ty\leq c^Tx$ for every feasible pair.

### Weak duality

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

Every feasible dual objective value bounds every feasible primal objective value.

#### Linear programming optimality certificate

↑ **Parent:** [Weak duality](#weak-duality)

For the [linear program](linear-programming.md) maximizing $c^Tx$ with $Ax\le b$, $x\ge0$, a vector $y\ge0$ with $A^Ty\ge c$ proves $c^Tx\le y^Tb$ for every feasible $x$. If a feasible $x$ attains that bound, it is optimal. This is [weak duality](#weak-duality) written as a directly checkable certificate; adding nonnegative multiples of constraints suffices to verify it. The equivalent reversed-inequality certificate applies to a minimization program.

#### Strong duality

↑ **Parent:** [Weak duality](#weak-duality)

Strong duality means that the primal and dual optimal values are equal. It holds for every feasible bounded [linear program](linear-programming.md) and for broad classes of [convex optimization](convex-optimization.md) problems under a constraint qualification.

##### Convex perturbation function

↑ **Parent:** [Strong duality](#strong-duality)

A jointly proper [convex function](real-analysis.md#convex-function) $f(x,z)$ represents an optimization problem at perturbation $z=0$ and a family of nearby problems at other $z$. Its primal value function is $p(z)=\inf_x f(x,z)$. Relaxing an inequality by $z$ gives the example $f(x,z)=J(x)+\delta_{(-\infty,0]}(r(x)-\sigma-z)$, using an [indicator functional](inverse-problem.md#indicator-functional-of-a-constraint-set). The resulting [convex perturbation duality](#convex-perturbation-duality) expresses multipliers as supporting [subgradients](real-analysis.md#subgradient) of the value function.

###### Convex perturbation duality

↑ **Parent:** [Convex perturbation function](#convex-perturbation-function)

For a [convex perturbation function](#convex-perturbation-function), define

$$
\varphi(x)=f(x,0),\qquad\psi(y)=-f^*(0,y),\qquad p(z)=\inf_x f(x,z),\qquad q(v)=\sup_y[-f^*(v,y)].
$$

The primal and dual values are $p(0)$ and $q(0)$; the signed dual marginal $q$ is concave. The identity $p^*(y)=f^*(0,y)$ gives $q(0)=p^{**}(0)$. If $p$ is proper and finite near zero, [subgradients](real-analysis.md#subgradient) at zero prove [strong duality](#strong-duality) with dual attainment. In finite dimensions the relative-interior condition $0\in\operatorname{ri}(\operatorname{dom}p)$ also suffices, provided $p(0)$ is finite. This does not itself prove primal attainment.

###### Sensitivity analysis in convex perturbation duality

↑ **Parent:** [Convex perturbation duality](#convex-perturbation-duality)

An optimal dual variable $y^*\in\partial p(0)$ bounds the effect of perturbing a convex value function:

$$
p(z)\geq p(0)+\langle y^*,z\rangle.
$$

If $p$ is finite convex near zero, $p'(0;d)=\max_{y\in\partial p(0)}\langle y,d\rangle$. A singleton [subdifferential](convex-optimization.md#subdifferential) gives differentiability and a first-order expansion. For an upper-bound constraint relaxed by $z$, the derivative equals the negative of the nonnegative [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier); relaxing the bound can decrease the minimum value.

<h5 id="slater-s-condition">Slater's condition</h5>

↑ **Parent:** [Strong duality](#strong-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slater's_condition)

The Slater condition requires a feasible point at which every nonlinear convex inequality is strict and every affine equality holds. For a convex problem it implies [strong duality](#strong-duality) and attainment of the dual optimum under standard finiteness assumptions.

##### Exact maximum-violation penalty

↑ **Parent:** [Strong duality](#strong-duality)

An exact maximum-violation penalty replaces inequalities $g_i(x)\leq0$ by the unconstrained objective $f(x)+M\max(0,g_1(x),\ldots,g_m(x))$. If an optimal dual multiplier is $\lambda^*$, every $M>\lVert\lambda^*\rVert_1$ makes every penalized minimizer feasible and optimal.

##### Dual attainment

↑ **Parent:** [Strong duality](#strong-duality)

[Dual attainment](#dual-attainment) means that a feasible choice of [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier) achieves the optimal value of the [Lagrangian dual problem](#lagrangian-dual-problem). Equality of primal and dual optimal values alone does not imply [dual attainment](#dual-attainment).

#### Duality gap

↑ **Parent:** [Weak duality](#weak-duality)

For finite primal and dual optimal values in a [minimization problem](mathematical-optimization.md#minimization-problem), the [duality gap](#duality-gap) is $p_*-d_*\geq0$. [Strong duality](#strong-duality) means this difference is zero.

### Complementary slackness

↑ **Parent:** [Linear programming duality](#linear-programming-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complementary_slackness)

At a primal-dual optimum, each positive variable corresponds to a tight dual constraint and conversely for positive dual variables.

### Transportation problem

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

The transportation problem minimizes linear shipping cost while matching prescribed row supplies and column demands.

This is the finite discrete [optimal transport](mathematical-optimization.md#optimal-transport) problem with prescribed supply and demand marginals.

#### Production costs in a transportation problem

↑ **Parent:** [Transportation problem](#transportation-problem)

When factory $i$ incurs unit production cost $p_i$ only on goods actually shipped, add that cost to every real shipping destination in its row. Unused capacity incurs no production cost; a dummy unused-capacity column therefore keeps zero cost rather than receiving $p_i$. This changes the optimal factory utilization when capacity exceeds total demand. [Transportation dual certificate with capacity inequalities](#transportation-dual-certificate-with-capacity-inequalities) proves optimality without assuming every factory must produce at full capacity.

#### Transportation dual potentials

↑ **Parent:** [Transportation problem](#transportation-problem)

Row and column potentials satisfying the displayed inequalities give a lower bound on the cost of every feasible shipment matrix: $\sum_{ij}c_{ij}x_{ij}\geq\sum_i u_i s_i+\sum_jv_j d_j$, since row sums are supplies $s_i$ and column sums are demands $d_j$. The [reduced costs](#reduced-cost) are $c_{ij}-u_i-v_j$. A feasible matrix using only zero-reduced-cost cells attains the lower bound, proving optimality by [weak duality](#weak-duality). The [transportation simplex algorithm](#transportation-simplex-algorithm) sets these potentials by equality on a [transportation spanning tree](#transportation-spanning-tree), and enters a negative-reduced-cost cell if one exists.

##### Transportation dual certificate with capacity inequalities

↑ **Parent:** [Transportation dual potentials](#transportation-dual-potentials)

For shipments $x_{ij}\geq0$ with factory row sums at most capacities $s_i$ and shop column sums exactly demands $d_j$, the displayed dual potentials give $\sum c_{ij}x_{ij}\geq\sum_i u_i s_i+\sum_jv_jd_j$. The sign $u_i\leq0$ ensures $u_i\sum_jx_{ij}\geq u_i s_i$. Equality proves optimality. It occurs when every used cell is tight and every row with spare capacity has $u_i=0$, the relevant [complementary slackness](#complementary-slackness) conditions. A dummy demand column with zero costs converts unused capacity into a balanced [transportation problem](#transportation-problem).

#### Assignment problem

↑ **Parent:** [Transportation problem](#transportation-problem)

The assignment problem chooses a one-to-one pairing of jobs and agents minimizing their total cost. Its [minimum-cost flow](graph-theory.md#minimum-cost-flow-problem) formulation puts unit supplies on job vertices and unit demands on agent vertices of a [bipartite graph](bipartite-graph.md). Integral feasible flows are [perfect matchings](matching-graph-theory.md#perfect-matching).

##### Assignment lower bound from independent task minima

↑ **Parent:** [Assignment problem](#assignment-problem)

For a partial [assignment problem](#assignment-problem), add its fixed cost to the sum, over remaining tasks, of each task's cheapest available machine cost. This is a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) because it relaxes the requirement that different tasks use distinct machines. It is an admissible bound for [branch and bound](mathematical-optimization.md#branch-and-bound), even though the minimizing choices may assign the same machine repeatedly.

// Target: mathematical-optimization.bigb

##### Hungarian algorithm

↑ **Parent:** [Assignment problem](#assignment-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hungarian_algorithm)

The Hungarian algorithm maintains feasible [assignment dual potentials](#assignment-dual-potentials) and a matching of equality edges. If the alternating search cannot augment, adjust reachable job and agent potentials by the smallest [reduced cost](#reduced-cost) leaving the search set. This preserves feasibility and existing matching equalities while exposing a new equality edge. A resulting [perfect matching](matching-graph-theory.md#perfect-matching) attains the dual lower bound.

##### Assignment dual potentials

↑ **Parent:** [Assignment problem](#assignment-problem)

These feasible potentials give the lower bound $\sum_i\lambda_i-\sum_j\mu_j$ on every assignment cost. An assignment using only equality edges attains this bound and is optimal by [weak duality](#weak-duality) and [complementary slackness](#complementary-slackness).

#### Transportation polytope

↑ **Parent:** [Transportation problem](#transportation-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transportation_polytope)

The transportation polytope is the set of nonnegative matrices with fixed row and column sums.

##### Transportation spanning tree

↑ **Parent:** [Transportation polytope](#transportation-polytope)

The positive cells of a nondegenerate transportation basis form a spanning tree in the bipartite graph of supply and demand vertices.

#### Transportation simplex algorithm

↑ **Parent:** [Transportation problem](#transportation-problem)

The transportation simplex computes row and column potentials, enters a negative-reduced-cost cell, and pivots around its induced alternating cycle.

##### Northwest corner method

↑ **Parent:** [Transportation simplex algorithm](#transportation-simplex-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Northwest_corner_method)

The northwest-corner method repeatedly allocates the smaller remaining supply and demand in the current top-left cell to construct an initial transportation basis.

##### Reduced cost

↑ **Parent:** [Transportation simplex algorithm](#transportation-simplex-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_cost)

For transportation potentials, the reduced cost is $\bar c_{ij}=c_{ij}-u_i-v_j$; a negative value identifies an improving entering cell.

##### Cycle pivot

↑ **Parent:** [Transportation simplex algorithm](#transportation-simplex-algorithm)

Adding a nonbasic edge to a transportation tree creates one cycle; alternating equal additions and subtractions around it preserves every row and column sum.

#### Integrality of the transportation problem

↑ **Parent:** [Transportation problem](#transportation-problem)

Integer supplies and demands admit an integer optimum because an integer initial basis and every cycle pivot remain integer.

##### Totally unimodular matrix

↑ **Parent:** [Integrality of the transportation problem](#integrality-of-the-transportation-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Totally_unimodular_matrix)

A matrix is totally unimodular when every square subdeterminant is $0$, $1$, or $-1$; linear programs with such a constraint matrix and integer right side have integral vertices.

## Simplex method

↑ **Parent:** [Linear programming](linear-programming.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplex_method)

The simplex method moves between adjacent [basic feasible solutions](#basic-feasible-solution) along improving edges of a feasible polytope until no improving pivot remains.

### Simplex optimality criterion

↑ **Parent:** [Simplex method](#simplex-method)

In a feasible minimization [simplex dictionary](numerical-analysis.md#simplex-dictionary), the nonbasic variables are nonnegative. If every [reduced cost](#reduced-cost) $\bar c_j\ge0$, the displayed objective identity proves $z\ge z_0$ for every feasible point. Thus the current [basic feasible solution](#basic-feasible-solution) is globally optimal. If all [reduced costs](#reduced-cost) are strictly positive, equality forces every nonbasic variable to vanish and gives a unique basic solution, provided the dictionary determines all basic variables.

### Greatest improvement pivot rule

↑ **Parent:** [Simplex method](#simplex-method)

For a feasible [simplex dictionary](numerical-analysis.md#simplex-dictionary), let $r_j>0$ be a nonbasic variable's improving [reduced cost](#reduced-cost) and let $\theta_j$ be its largest feasible increase from the [simplex ratio test](#simplex-ratio-test). The [greatest improvement pivot rule](#greatest-improvement-pivot-rule) chooses an entering variable maximizing $r_j\theta_j$. It measures the improvement over the entire edge, whereas the [Dantzig pivot rule](#dantzig-pivot-rule) maximizes only $r_j$.

// Target: mathematical-optimization.bigb

### Dantzig pivot rule

↑ **Parent:** [Simplex method](#simplex-method)

In maximization, select the entering nonbasic variable with greatest positive [reduced cost](#reduced-cost), meaning objective increase per unit of that variable. Unlike geometric steepest-edge pricing, this rate depends on variable and constraint scaling. A rescaled [Klee-Minty cube](#klee-minty-cube) can give the same $2^n-1$-pivot path as smallest-index improving-facet pivoting.

### Klee-Minty cube

↑ **Parent:** [Simplex method](#simplex-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klee–Minty_cube)

For $0<\varepsilon<1/2$, these inequalities define a deformed [cube](euclidean-geometry.md#cube) with $2^n$ [vertices of a polytope](convex-set.md#vertex-of-a-polytope). Choose either the lower or upper bound recursively at each coordinate to obtain a [vertex of a polytope](convex-set.md#vertex-of-a-polytope); changing one choice gives an adjacent [vertex of a polytope](convex-set.md#vertex-of-a-polytope). When maximizing $x_n$, smallest-index improving-facet pivoting visits all $2^n$ [vertices of a polytope](convex-set.md#vertex-of-a-polytope): first traverse the lower last-coordinate face, then move to the upper face and traverse the preceding path in reverse. Thus this geometric version of the [Bland pivoting rule](#bland-pivoting-rule) can require $2^n-1$ pivots. Rescaling the coordinate $x_i$ to $y_i=\varepsilon^{2(n-i)}x_i$ makes the positive rate per unit freed coordinate equal to $\varepsilon^{-(n-i)}$; [Dantzig pivot rule](#dantzig-pivot-rule) then selects the same exponential path. Euclidean edge-length pricing is a different rule.

### Simplex tableau

↑ **Parent:** [Simplex method](#simplex-method)

A simplex tableau records the canonical constraint equations for a [simplex basis](#simplex-basis) and the canonical objective equation. For maximization use $z+\sum_j\rho_jx_j=z_0$, so a negative nonbasic objective-row coefficient is an improving direction. Constraint rows have an identity matrix in the basic columns. A [simplex method](#simplex-method) pivot divides the leaving row by the pivot coefficient and eliminates the entering column from the other rows, including the objective row. The [simplex ratio test](#simplex-ratio-test) chooses the largest feasible step. When all basic values and all $\rho_j$ are nonnegative, the objective equation directly proves $z\leq z_0$ for every nonnegative feasible vector.

#### Reconstructing a linear program from a final simplex tableau

↑ **Parent:** [Simplex tableau](#simplex-tableau)

For a maximization problem with unpriced unit [slack variables](#slack-variable), their columns in a final [simplex tableau](#simplex-tableau) give $B^{-1}$, where $B$ consists of the original basic columns. The constraint right side is $\bar b=B^{-1}b$, so $b=B\bar b$. If the objective row uses [reduced costs](#reduced-cost) $r_j=c_j-c_B^TB^{-1}A_j$, its slack entries are $-y^T$ with $y^T=c_B^TB^{-1}$. Therefore $c_B^T=y^TB$. In a homogeneous linear objective with no constant offset, the displayed basic objective value must equal $c_B^T\bar b=y^Tb$. This identity detects inconsistent tableau constants; an affine offset affects the value but not the reduced costs.

#### Simplex objective update for a priced slack variable

↑ **Parent:** [Simplex tableau](#simplex-tableau)

If a variable $x_k$ gains an objective coefficient $p$, the new objective is $z=z_{\rm old}+px_k$. Substitute this in the old canonical objective equation and eliminate any remaining basic-column coefficients using the constraint rows. If $x_k$ is nonbasic, this simply subtracts $p$ from its objective-row coefficient. When a [slack variable](#slack-variable) is sold, rename the old slack as the sales quantity; its equation already gives the correct equality and no new slack is added. Reoptimization can then start directly from the altered [simplex tableau](#simplex-tableau).

### Bland pivoting rule

↑ **Parent:** [Simplex method](#simplex-method)

For a maximization [simplex dictionary](numerical-analysis.md#simplex-dictionary), choose the smallest-index nonbasic variable with positive reduced cost to enter. Among basic variables attaining the minimum feasible ratio, choose the smallest-index one to leave. This fixed index rule prevents cycling, including in degenerate pivots whose step length is zero. It need not minimize the number of pivots on a particular instance.

### Two-phase simplex

↑ **Parent:** [Simplex method](#simplex-method)

Phase I introduces nonnegative artificial variables to create a feasible basis and minimizes their sum, or maximizes its negative. A positive minimum proves infeasibility. At a zero minimum, remove artificial variables and use the resulting feasible original basis in Phase II with the original objective. If an artificial variable remains basic at zero, pivot it out when possible; otherwise its row is redundant. Each phase uses the [simplex ratio test](#simplex-ratio-test) to preserve nonnegative basic values.

### Simplex ratio test

↑ **Parent:** [Simplex method](#simplex-method)

In a feasible [simplex basis](#simplex-basis), increasing a nonbasic variable by $\theta$ changes basic coordinates to $x-\theta d$. Nonnegativity limits $\theta$ by the smallest ratio $x_i/d_i$ with $d_i>0$; a minimizing coordinate leaves the basis. Ties can leave zero-valued basic variables. This pivot test is distinct from the analytic [ratio test](sequence-and-series.md#ratio-test) for series convergence.

### Simplex basis

↑ **Parent:** [Simplex method](#simplex-method)

For standard-form [linear programming](linear-programming.md) constraints $Ax=b$ of full row rank, a simplex basis is a set of columns forming an invertible square matrix $B$. The remaining variables are nonbasic; setting them to zero gives the basic solution $x_B=B^{-1}b$. It is feasible if these basic variables are nonnegative. A pivot exchanges one basic and one nonbasic column while maintaining this representation.

#### Nonbasic variable

↑ **Parent:** [Simplex basis](#simplex-basis)

A [nonbasic variable](#nonbasic-variable) corresponds to a column outside the current [simplex basis](#simplex-basis). In standard nonnegative [linear programming](linear-programming.md), it is set to zero at the basic solution. With explicit finite bounds, it is normally fixed at one of its bounds.

// Target: mathematical-optimization.bigb

#### Basic variable

↑ **Parent:** [Simplex basis](#simplex-basis)

A [basic variable](#basic-variable) corresponds to a column of the current [simplex basis](#simplex-basis). Given the nonbasic variables, the invertible basis matrix determines the basic variables from the equality constraints.

// Target: mathematical-optimization.bigb

#### Linear programming sensitivity within a fixed optimal basis

↑ **Parent:** [Simplex basis](#simplex-basis)

For a [linear program](linear-programming.md) with unchanged cost and constraint matrix, an optimal [simplex basis](#simplex-basis) remains optimal while its basic solution remains feasible. Its [reduced costs](#reduced-cost) and dual certificate do not change. The new basic variables are $A_B^{-1}(b+\epsilon)$, and the objective is the displayed affine function, with $y$ the basis's dual solution. This gives an exact piecewise-affine sensitivity region, determined by nonnegativity of the basic variables, rather than merely a formal first derivative.

##### Strictly positive dual certificate and right-hand-side sensitivity

↑ **Parent:** [Linear programming sensitivity within a fixed optimal basis](#linear-programming-sensitivity-within-a-fixed-optimal-basis)

For a square invertible constraint matrix $A$ in $\max\{c^Tx:Ax\leq b,x\geq0\}$, suppose $y>0$ and $A^Ty=c$. This fixed dual vector stays optimal under a changed right-hand side $b'$ exactly when $A^{-1}b'\geq0$. Sufficiency follows from primal feasibility and equal primal/dual objectives. Necessity follows from [complementary slackness](#complementary-slackness): since every $y_i$ is positive, every optimal primal constraint must bind, forcing $x=A^{-1}b'$. The inequalities define the whole validity cone, including degenerate boundary optima.

### Simplex paths on a cube with one truncated corner

↑ **Parent:** [Simplex method](#simplex-method)

For $0\leq x_i\leq1$, $x_1+x_2+x_3\leq5/2$, and objective $x_1+2x_2+4x_3$, the oriented edge graph has eight improving paths from the origin to the unique optimum $(1/2,1,1)$. Their lengths range from three to five pivots.

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (19)

- [Contact time of translating line segments](convex-set.md#contact-time-of-translating-line-segments)
- [Critical path method](mathematical-optimization.md#critical-path-method)
- [Exact linear optimization from a feasibility oracle](#exact-linear-optimization-from-a-feasibility-oracle)
- [Fractional knapsack problem](mathematical-optimization.md#fractional-knapsack-problem)
- [Karmarkar standard form](#karmarkar-standard-form)
- [Linear optimization on a convex hull](convex-set.md#linear-optimization-on-a-convex-hull)
- [Nonbasic variable](#nonbasic-variable)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3.md#12g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-40.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38.md#2/b/solution)
- [Project scheduling duality](mathematical-optimization.md#project-scheduling-duality)
- [Semidefinite programming](convex-optimization.md#semidefinite-programming)
- [Simplex basis](#simplex-basis)
