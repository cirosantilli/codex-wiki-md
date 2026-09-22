# Mathematical optimization

↑ **Parent:** [Area of mathematics](mathematics.md#area-of-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mathematical_optimization)

Mathematical optimization studies extrema under constraints.

**Table of contents**

- [Scheduling](#scheduling)
  - [Parallel-machine makespan with sequence-dependent setups](#parallel-machine-makespan-with-sequence-dependent-setups)
- [Objective function](#objective-function)
- [Project scheduling](#project-scheduling)
  - [Critical path method](#critical-path-method)
    - [Project scheduling duality](#project-scheduling-duality)
      - [Unit-flow certificate for project duration](#unit-flow-certificate-for-project-duration)
- [Maximum and minimum](#maximum-and-minimum)
- [Cobb–Douglas production function](#cobb-douglas-production-function)
- [Heuristic optimization](#heuristic-optimization)
  - [Tabu search](#tabu-search)
  - [Simulated annealing](#simulated-annealing)
    - [Likelihood-power annealing](#likelihood-power-annealing)
      - [Binomial likelihood-power annealing](#binomial-likelihood-power-annealing)
      - [Gaussian likelihood Gibbs annealing](#gaussian-likelihood-gibbs-annealing)
  - [Local search](#local-search)
- [Feasible point](#feasible-point)
- [Nonlinear programming](#nonlinear-programming)
- [Perturbation function](#perturbation-function)
- [Chance constraint](#chance-constraint)
  - [Deterministic boundary in an upper-tail chance constraint](#deterministic-boundary-in-an-upper-tail-chance-constraint)
  - [Exact Gaussian chance constraint](#exact-gaussian-chance-constraint)
- [Variational inequality](#variational-inequality)
- [First-order optimality condition](#first-order-optimality-condition)
- [Lagrangian duality](#lagrangian-duality)
  - [Strong Lagrangian property](#strong-lagrangian-property)
  - [Primal problem](#primal-problem)
- [Maximization problem](#maximization-problem)
- [Minimization problem](#minimization-problem)
- [Parametric optimization](#parametric-optimization)
  - [Solution map of a parametric optimization problem](#solution-map-of-a-parametric-optimization-problem)
- [Variational analysis](#variational-analysis)
  - [Normal cone](#normal-cone)
    - [Limiting normal cone](#limiting-normal-cone)
    - [Fréchet normal cone](#frechet-normal-cone)
  - [Set-valued analysis](#set-valued-analysis)
    - [Set-valued mapping](#set-valued-mapping)
      - [Upper hemicontinuity](#upper-hemicontinuity)
      - [Aubin property](#aubin-property)
        - [Mordukhovich criterion](#mordukhovich-criterion)
      - [Graph of a set-valued mapping](#graph-of-a-set-valued-mapping)
        - [Limiting coderivative](#limiting-coderivative)
- [Pareto efficiency](#pareto-efficiency)
  - [Pairwise improvement from nonparallel utility gradients](#pairwise-improvement-from-nonparallel-utility-gradients)
  - [Pareto frontier](#pareto-frontier)
- [Approximation algorithm](#approximation-algorithm)
  - [Fully polynomial randomized approximation scheme](#fully-polynomial-randomized-approximation-scheme)
  - [Fully polynomial-time approximation scheme](#fully-polynomial-time-approximation-scheme)
  - [Approximation ratio](#approximation-ratio)
    - [Relative-error approximation for minimization](#relative-error-approximation-for-minimization)
- [Integer programming](#integer-programming)
  - [Two-bin load balancing](#two-bin-load-balancing)
    - [Rounded dynamic programming for two-bin load balancing](#rounded-dynamic-programming-for-two-bin-load-balancing)
    - [Greedy two-bin scheduling bound](#greedy-two-bin-scheduling-bound)
  - [Small integer feasibility witness by homogeneous cone decomposition](#small-integer-feasibility-witness-by-homogeneous-cone-decomposition)
  - [Winner determination problem](#winner-determination-problem)
    - [Greedy half-approximation for submodular welfare](#greedy-half-approximation-for-submodular-welfare)
  - [Quadratic assignment problem](#quadratic-assignment-problem)
    - [Gilmore-Lawler bound](#gilmore-lawler-bound)
  - [Branch and bound](#branch-and-bound)
    - [Incumbent solution](#incumbent-solution)
    - [Best-bound search](#best-bound-search)
  - [Knapsack problem](#knapsack-problem)
    - [Quadratic knapsack problem](#quadratic-knapsack-problem)
      - [Fractional row bound for quadratic knapsack](#fractional-row-bound-for-quadratic-knapsack)
    - [Fractional knapsack problem](#fractional-knapsack-problem)
    - [0-1 knapsack problem](#0-1-knapsack-problem)
      - [Half-approximation algorithm for knapsack](#half-approximation-algorithm-for-knapsack)
  - [Cutting-plane method](#cutting-plane-method)
    - [Gomory fractional cut](#gomory-fractional-cut)
      - [Gomory infeasibility certificate from a fractional slack row](#gomory-infeasibility-certificate-from-a-fractional-slack-row)
- [Travelling salesman problem](#travelling-salesman-problem)
  - [Assignment relaxation of the travelling salesman problem](#assignment-relaxation-of-the-travelling-salesman-problem)
  - [2-opt](#2-opt)
    - [Asymmetric 2-opt reversal cost](#asymmetric-2-opt-reversal-cost)
  - [Dummy-job reduction for sequence-dependent setup times](#dummy-job-reduction-for-sequence-dependent-setup-times)
  - [Subtour elimination constraints](#subtour-elimination-constraints)
  - [Compact order formulation of the travelling salesman problem](#compact-order-formulation-of-the-travelling-salesman-problem)
  - [Max-TSP](#max-tsp)
    - [Cycle-cover patching half-approximation for Max-TSP](#cycle-cover-patching-half-approximation-for-max-tsp)
  - [Metric travelling salesman problem](#metric-travelling-salesman-problem)
    - [Double-tree approximation for metric TSP](#double-tree-approximation-for-metric-tsp)
    - [Christofides algorithm](#christofides-algorithm)
  - [Euclidean travelling salesman tour](#euclidean-travelling-salesman-tour)
    - [Weighted mismatch bound for Euclidean tours](#weighted-mismatch-bound-for-euclidean-tours)
    - [Squared edge bound for tours in the unit square](#squared-edge-bound-for-tours-in-the-unit-square)
      - [Quadratic path bound in a right triangle](#quadratic-path-bound-in-a-right-triangle)
- [Randomized rounding](#randomized-rounding)
  - [Gaussian hyperplane rounding](#gaussian-hyperplane-rounding)
    - [Krivine rounding scheme](#krivine-rounding-scheme)
      - [Bipartite sign rounding bound](#bipartite-sign-rounding-bound)
      - [Krivine rounding constant](#krivine-rounding-constant)
- [Quadratic optimization](#quadratic-optimization)
  - [Quadratic program](#quadratic-program)
  - [Binary quadratic optimization](#binary-quadratic-optimization)
    - [Bipartite binary quadratic optimization](#bipartite-binary-quadratic-optimization)
- [Optimal transport](#optimal-transport)
  - [c-cyclical monotonicity](#c-cyclical-monotonicity)
    - [Finite-cost optimal transport converse](#finite-cost-optimal-transport-converse)
    - [Strong c-monotonicity](#strong-c-monotonicity)
      - [Symmetric clipping proof of transport optimality](#symmetric-clipping-proof-of-transport-optimality)
      - [Transport potential path construction](#transport-potential-path-construction)
  - [Monotone rearrangement](#monotone-rearrangement)
    - [One-dimensional quadratic transport uniqueness criterion](#one-dimensional-quadratic-transport-uniqueness-criterion)
  - [Knott–Smith optimality criterion](#knott-smith-optimality-criterion)
    - [Brenier theorem](#brenier-theorem)
  - [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem)
    - [Transport cost function](#transport-cost-function)
    - [Kantorovich duality theorem](#kantorovich-duality-theorem)
      - [Kantorovich duality by positive extension](#kantorovich-duality-by-positive-extension)
      - [Kantorovich potential](#kantorovich-potential)
    - [Transport plan](#transport-plan)
  - [Monge optimal transport problem](#monge-optimal-transport-problem)
    - [Transport map](#transport-map)
      - [Measure-preserving parametrization of one-dimensional transport maps](#measure-preserving-parametrization-of-one-dimensional-transport-maps)
- [Lagrange sufficiency theorem](#lagrange-sufficiency-theorem)
  - [Minimum squared norm under two affine constraints](#minimum-squared-norm-under-two-affine-constraints)
  - [Scalar multiplier certificate for a quadratic equality constraint](#scalar-multiplier-certificate-for-a-quadratic-equality-constraint)
- [Dynamic programming](#dynamic-programming)
  - [Dynamic programming principle](#dynamic-programming-principle)
  - [Average-reward optimal policy](#average-reward-optimal-policy)
    - [Average-reward Bellman equation](#average-reward-bellman-equation)
  - [Control policy](#control-policy)
    - [Markov policy](#markov-policy)
  - [Retirement threshold with multiplicative capture risk](#retirement-threshold-with-multiplicative-capture-risk)
  - [Bellman equation](#bellman-equation)
    - [Dynamic programming operator](#dynamic-programming-operator)
    - [Bellman comparison with nonnegative rewards and superunit discount](#bellman-comparison-with-nonnegative-rewards-and-superunit-discount)
    - [Hamilton-Jacobi-Bellman equation](#hamilton-jacobi-bellman-equation)
      - [Verification by a nonnegative control supermartingale](#verification-by-a-nonnegative-control-supermartingale)
      - [Linear-quadratic optimal control](#linear-quadratic-optimal-control)
        - [Discrete Riccati recurrence](#discrete-riccati-recurrence)
  - [Value function](#value-function)
    - [Non-vertical supporting hyperplane of a value function](#non-vertical-supporting-hyperplane-of-a-value-function)
  - [Bayesian box search problem](#bayesian-box-search-problem)
    - [Optimal index for Bayesian box search](#optimal-index-for-bayesian-box-search)
    - [Rewarded Bayesian box search Bellman equation](#rewarded-bayesian-box-search-bellman-equation)
- [Newton's method in optimization](#newton-s-method-in-optimization)
  - [Quadratic convergence bound for Newton's method](#quadratic-convergence-bound-for-newton-s-method)
- [Karush-Kuhn-Tucker conditions](#karush-kuhn-tucker-conditions)
  - [Active-set transition in capped resource allocation](#active-set-transition-in-capped-resource-allocation)
- [Convex optimization](convex-optimization.md)
  - [Pari-mutuel expected-return allocation](convex-optimization.md#pari-mutuel-expected-return-allocation)
  - [Separation oracle](convex-optimization.md#separation-oracle)
    - [Path-constraint separation by shortest paths](convex-optimization.md#path-constraint-separation-by-shortest-paths)
  - [Chambolle–Pock algorithm](convex-optimization.md#chambolle-pock-algorithm)
    - [Convergence of primal-dual hybrid gradient](convex-optimization.md#convergence-of-primal-dual-hybrid-gradient)
  - [Convex positively one-homogeneous functional](convex-optimization.md#convex-positively-one-homogeneous-functional)
    - [Generalized eigenfunction in the forward-operator metric](convex-optimization.md#generalized-eigenfunction-in-the-forward-operator-metric)
  - [Conic optimization](convex-optimization.md#conic-optimization)
    - [Farkas' lemma](convex-optimization.md#farkas-lemma)
      - [Robust infeasibility under uniform constraint relaxation](convex-optimization.md#robust-infeasibility-under-uniform-constraint-relaxation)
      - [Farkas certificate for linear inequalities](convex-optimization.md#farkas-certificate-for-linear-inequalities)
        - [Normalized integer Farkas infeasibility gap](convex-optimization.md#normalized-integer-farkas-infeasibility-gap)
    - [Interior-point method](convex-optimization.md#interior-point-method)
      - [Homogeneous self-dual embedding of a linear program](convex-optimization.md#homogeneous-self-dual-embedding-of-a-linear-program)
      - [Conic phase-I problem](convex-optimization.md#conic-phase-i-problem)
      - [Self-concordant barrier](convex-optimization.md#self-concordant-barrier)
        - [Logarithmically homogeneous barrier](convex-optimization.md#logarithmically-homogeneous-barrier)
          - [Legendre dual cone barrier](convex-optimization.md#legendre-dual-cone-barrier)
        - [Dikin ellipsoid](convex-optimization.md#dikin-ellipsoid)
        - [Central path](convex-optimization.md#central-path)
          - [Central-path Newton system](convex-optimization.md#central-path-newton-system)
    - [Conic dual problem](convex-optimization.md#conic-dual-problem)
    - [Completely positive optimization](convex-optimization.md#completely-positive-optimization)
    - [Copositive optimization](convex-optimization.md#copositive-optimization)
      - [Copositive reformulation of an orthant Rayleigh minimum](convex-optimization.md#copositive-reformulation-of-an-orthant-rayleigh-minimum)
  - [Robust optimization](convex-optimization.md#robust-optimization)
    - [Robust linear optimization over the probability simplex](convex-optimization.md#robust-linear-optimization-over-the-probability-simplex)
    - [Polyhedral uncertainty set](convex-optimization.md#polyhedral-uncertainty-set)
  - [Convex analysis](convex-optimization.md#convex-analysis)
    - [Infimal convolution](convex-optimization.md#infimal-convolution)
      - [Finite-valued infimal convolution](convex-optimization.md#finite-valued-infimal-convolution)
        - [Infimal-convolution dual subgradients](convex-optimization.md#infimal-convolution-dual-subgradients)
      - [Conjugate of an infimal convolution](convex-optimization.md#conjugate-of-an-infimal-convolution)
  - [Proportional fairness](convex-optimization.md#proportional-fairness)
    - [Inactive routes in proportional fairness](convex-optimization.md#inactive-routes-in-proportional-fairness)
    - [Proportionally fair allocation on a four-cycle](convex-optimization.md#proportionally-fair-allocation-on-a-four-cycle)
      - [Opposite-route reduction for a proportionally fair four-cycle](convex-optimization.md#opposite-route-reduction-for-a-proportionally-fair-four-cycle)
    - [Weighted logarithmic utility](convex-optimization.md#weighted-logarithmic-utility)
  - [Semidefinite programming](convex-optimization.md#semidefinite-programming)
    - [Semidefinite relaxation of binary quadratic optimization](convex-optimization.md#semidefinite-relaxation-of-binary-quadratic-optimization)
    - [Semidefinite relaxation of slab-constrained quadratic maximization](convex-optimization.md#semidefinite-relaxation-of-slab-constrained-quadratic-maximization)
      - [Rademacher rounding for a semidefinite relaxation](convex-optimization.md#rademacher-rounding-for-a-semidefinite-relaxation)
        - [Logarithmic approximation bound for slab-constrained quadratic maximization](convex-optimization.md#logarithmic-approximation-bound-for-slab-constrained-quadratic-maximization)
  - [Water-filling algorithm](convex-optimization.md#water-filling-algorithm)
    - [Logarithmic water filling](convex-optimization.md#logarithmic-water-filling)
  - [Coordinate descent](convex-optimization.md#coordinate-descent)
  - [Convex conjugate](convex-optimization.md#convex-conjugate)
    - [Utility conjugate](convex-optimization.md#utility-conjugate)
      - [Dual differentiability with nonvanishing utility curvature](convex-optimization.md#dual-differentiability-with-nonvanishing-utility-curvature)
    - [Convex conjugate of x log x](convex-optimization.md#convex-conjugate-of-x-log-x)
    - [Biconjugate](convex-optimization.md#biconjugate)
    - [Affine covariance of the convex conjugate](convex-optimization.md#affine-covariance-of-the-convex-conjugate)
    - [Concave Legendre dual](convex-optimization.md#concave-legendre-dual)
      - [Lower conjugate](convex-optimization.md#lower-conjugate)
        - [Concave biconjugate](convex-optimization.md#concave-biconjugate)
      - [Inverse-flux quadratic bounds](convex-optimization.md#inverse-flux-quadratic-bounds)
    - [Convex conjugate of a constrained quadratic](convex-optimization.md#convex-conjugate-of-a-constrained-quadratic)
    - [Fenchel-Moreau theorem](convex-optimization.md#fenchel-moreau-theorem)
      - [Biconjugation as closed convexification](convex-optimization.md#biconjugation-as-closed-convexification)
    - [Fenchel–Young inequality](convex-optimization.md#fenchel-young-inequality)
      - [Fenchel–Young gap](convex-optimization.md#fenchel-young-gap)
  - [Subdifferential](convex-optimization.md#subdifferential)
    - [Fermat rule for convex minimization](convex-optimization.md#fermat-rule-for-convex-minimization)
    - [Monotonicity of a convex subdifferential](convex-optimization.md#monotonicity-of-a-convex-subdifferential)
    - [Forward subgradient step](convex-optimization.md#forward-subgradient-step)
    - [Partial subdifferential](convex-optimization.md#partial-subdifferential)
    - [Subgradient inversion under convex conjugacy](convex-optimization.md#subgradient-inversion-under-convex-conjugacy)
    - [Subdifferential under scalar affine composition](convex-optimization.md#subdifferential-under-scalar-affine-composition)
    - [Subdifferential of the L1 norm](convex-optimization.md#subdifferential-of-the-l1-norm)
    - [Subdifferential sum rule](convex-optimization.md#subdifferential-sum-rule)
  - [Absolutely one-homogeneous functional](convex-optimization.md#absolutely-one-homogeneous-functional)
    - [Generalized singular vector](convex-optimization.md#generalized-singular-vector)
    - [Euler identity for a convex one-homogeneous functional](convex-optimization.md#euler-identity-for-a-convex-one-homogeneous-functional)
    - [Eigenfunction of an absolutely one-homogeneous functional](convex-optimization.md#eigenfunction-of-an-absolutely-one-homogeneous-functional)
  - [Stiemke theorem](convex-optimization.md#stiemke-theorem)
  - [Projected gradient descent](convex-optimization.md#projected-gradient-descent)
    - [Projected subgradient method](convex-optimization.md#projected-subgradient-method)
    - [Averaged projected-gradient bound](convex-optimization.md#averaged-projected-gradient-bound)
  - [Step size](convex-optimization.md#step-size)
  - [Proximal operator](convex-optimization.md#proximal-operator)
    - [Radial soft thresholding](convex-optimization.md#radial-soft-thresholding)
    - [Banach-space proximal minimization](convex-optimization.md#banach-space-proximal-minimization)
    - [Proximal operator under affine rescaling](convex-optimization.md#proximal-operator-under-affine-rescaling)
    - [Moreau envelope](convex-optimization.md#moreau-envelope)
      - [Moreau envelope of the Euclidean norm](convex-optimization.md#moreau-envelope-of-the-euclidean-norm)
      - [Gradient of a Moreau envelope](convex-optimization.md#gradient-of-a-moreau-envelope)
      - [Moreau smoothing of a negative log-density](convex-optimization.md#moreau-smoothing-of-a-negative-log-density)
      - [Squared distance to a convex set](convex-optimization.md#squared-distance-to-a-convex-set)
        - [Conjugate of the squared distance to a convex set](convex-optimization.md#conjugate-of-the-squared-distance-to-a-convex-set)
    - [Moreau decomposition](convex-optimization.md#moreau-decomposition)
      - [Proximal operator of a support function](convex-optimization.md#proximal-operator-of-a-support-function)
    - [Proximal gradient method](convex-optimization.md#proximal-gradient-method)
      - [Alternating proximal-gradient operator](convex-optimization.md#alternating-proximal-gradient-operator)
        - [Implicit nonsmooth block in alternating proximal-gradient iteration](convex-optimization.md#implicit-nonsmooth-block-in-alternating-proximal-gradient-iteration)
        - [Mixed-point norm identity for alternating updates](convex-optimization.md#mixed-point-norm-identity-for-alternating-updates)
      - [Iterative soft-thresholding algorithm](convex-optimization.md#iterative-soft-thresholding-algorithm)
  - [Subgradient method](convex-optimization.md#subgradient-method)
  - [Log-sum-exp function](convex-optimization.md#log-sum-exp-function)
    - [Smooth maximum](convex-optimization.md#smooth-maximum)
  - [Nesterov accelerated gradient method](convex-optimization.md#nesterov-accelerated-gradient-method)
  - [Monotone operator](convex-optimization.md#monotone-operator)
    - [Cocoercivity](convex-optimization.md#cocoercivity)
      - [Baillon–Haddad theorem](convex-optimization.md#baillon-haddad-theorem)
    - [Resolvent of a monotone operator](convex-optimization.md#resolvent-of-a-monotone-operator)
    - [Maximal monotone operator](convex-optimization.md#maximal-monotone-operator)
    - [Nonexpansive mapping](convex-optimization.md#nonexpansive-mapping)
      - [Averaged operator](convex-optimization.md#averaged-operator)
        - [Browder convergence theorem for averaged operators](convex-optimization.md#browder-convergence-theorem-for-averaged-operators)
        - [Averaged-operator inequality](convex-optimization.md#averaged-operator-inequality)
    - [Firmly nonexpansive mapping](convex-optimization.md#firmly-nonexpansive-mapping)
    - [Proximal point algorithm](convex-optimization.md#proximal-point-algorithm)
      - [Douglas–Rachford method](convex-optimization.md#douglas-rachford-method)
        - [Product-space reformulation of convex feasibility](convex-optimization.md#product-space-reformulation-of-convex-feasibility)
      - [Preconditioned proximal point algorithm](convex-optimization.md#preconditioned-proximal-point-algorithm)
  - [Primal-dual optimal point](convex-optimization.md#primal-dual-optimal-point)
  - [Equality-constrained convex optimization](convex-optimization.md#equality-constrained-convex-optimization)
  - [Proximal gradient methods for learning](convex-optimization.md#proximal-gradient-methods-for-learning)
- [Lagrange multiplier](#lagrange-multiplier)
  - [Maximum box volume in an ellipsoid](#maximum-box-volume-in-an-ellipsoid)
  - [Minimum-area closed cylinder at fixed volume](#minimum-area-closed-cylinder-at-fixed-volume)
  - [Envelope theorem](#envelope-theorem)
  - [Optimization Lagrangian](#optimization-lagrangian)
  - [Derivative of a constrained value function](#derivative-of-a-constrained-value-function)
  - [Weighted open-box minimization](#weighted-open-box-minimization)
- [Arithmetic-geometric mean inequality](#arithmetic-geometric-mean-inequality)
- [Linear programming](#linear-programming)
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
- [Convex set](#convex-set)
  - [Hyperplane separation theorem](#hyperplane-separation-theorem)
  - [Supporting hyperplane theorem](#supporting-hyperplane-theorem)
  - [Relative interior](#relative-interior)
  - [Radially open convex set](#radially-open-convex-set)
  - [Half-space representation of a closed convex set](#half-space-representation-of-a-closed-convex-set)
  - [Recession cone](#recession-cone)
  - [Face of a convex set](#face-of-a-convex-set)
  - [Compact convex set](#compact-convex-set)
  - [Nonnegative orthant](#nonnegative-orthant)
  - [Convex combination](#convex-combination)
    - [Cyclic symmetry averaging](#cyclic-symmetry-averaging)
  - [Closed half-space](#closed-half-space)
  - [Line segment](#line-segment)
    - [Midpoint](#midpoint)
    - [Closest points on two line segments](#closest-points-on-two-line-segments)
      - [Contact time of translating line segments](#contact-time-of-translating-line-segments)
        - [Proximity time of translating line segments](#proximity-time-of-translating-line-segments)
  - [Convex polytope](#convex-polytope)
    - [Zonotope](#zonotope)
    - [Lattice polytope](#lattice-polytope)
    - [Convex polygon](#convex-polygon)
      - [Convex chain](#convex-chain)
        - [Convex-chain probability in a triangle](#convex-chain-probability-in-a-triangle)
        - [Longest convex chain](#longest-convex-chain)
          - [Convex-chain median concentration](#convex-chain-median-concentration)
    - [Vertex of a polytope](#vertex-of-a-polytope)
    - [Facet](#facet)
      - [Facet lower bound for ball approximations](#facet-lower-bound-for-ball-approximations)
    - [Cross-polytope](#cross-polytope)
  - [Extreme point](#extreme-point)
    - [Extreme points of real sequence-space unit balls](#extreme-points-of-real-sequence-space-unit-balls)
    - [Extreme points of a real continuous-function unit ball](#extreme-points-of-a-real-continuous-function-unit-ball)
      - [Clopen sign approximation in the real Cantor unit ball](#clopen-sign-approximation-in-the-real-cantor-unit-ball)
    - [Extreme-point criterion for the L-infinity unit ball](#extreme-point-criterion-for-the-l-infinity-unit-ball)
  - [Projections onto convex sets](#projections-onto-convex-sets)
  - [Euclidean projection onto a convex set](#euclidean-projection-onto-a-convex-set)
    - [Variational characterization of convex projection](#variational-characterization-of-convex-projection)
    - [Nonexpansiveness of metric projection](#nonexpansiveness-of-metric-projection)
    - [Projection onto a box-constrained hyperplane](#projection-onto-a-box-constrained-hyperplane)
  - [Support function](#support-function)
    - [Support-function subgradients as exposed faces](#support-function-subgradients-as-exposed-faces)
    - [Support function of an inverse image of an infinity-norm ball](#support-function-of-an-inverse-image-of-an-infinity-norm-ball)
    - [Sum of the largest components](#sum-of-the-largest-components)
      - [Threshold formula for the sum of the largest components](#threshold-formula-for-the-sum-of-the-largest-components)
    - [Sum of the largest eigenvalues](#sum-of-the-largest-eigenvalues)
      - [Ky Fan maximum principle](#ky-fan-maximum-principle)
        - [Hermitian effect variational principle](#hermitian-effect-variational-principle)
      - [Threshold semidefinite program for the largest eigenvalues](#threshold-semidefinite-program-for-the-largest-eigenvalues)
  - [Capped simplex](#capped-simplex)
  - [Second-order cone](#second-order-cone)
    - [Self-duality of a second-order cone](#self-duality-of-a-second-order-cone)
    - [Second-order cone programming](#second-order-cone-programming)
      - [Second-order cone reformulation of one-sided quadratic denoising](#second-order-cone-reformulation-of-one-sided-quadratic-denoising)
    - [Projection onto the second-order cone](#projection-onto-the-second-order-cone)
  - [Convex hull](#convex-hull)
    - [Closed convex hull](#closed-convex-hull)
    - [Carathéodory's theorem (convex hull)](#caratheodory-s-theorem-convex-hull)
      - [Conic Carathéodory theorem](#conic-caratheodory-theorem)
  - [Convex cone](#convex-cone)
    - [Orthant](#orthant)
    - [Strictly positive barycentre cone lemma](#strictly-positive-barycentre-cone-lemma)
      - [Positive-weight expectation cone](#positive-weight-expectation-cone)
    - [Support-minimal rays of a nonnegative kernel](#support-minimal-rays-of-a-nonnegative-kernel)
    - [Lineality space](#lineality-space)
    - [Self-dual cone](#self-dual-cone)
    - [Proper cone](#proper-cone)
    - [Completely positive cone](#completely-positive-cone)
      - [Closedness of the completely positive cone](#closedness-of-the-completely-positive-cone)
    - [Pointed cone](#pointed-cone)
    - [Closed convex cone](#closed-convex-cone)
      - [Separation from a closed convex cone](#separation-from-a-closed-convex-cone)
    - [Conic hull](#conic-hull)
      - [Finitely generated cone](#finitely-generated-cone)
        - [Closedness of finitely generated cones](#closedness-of-finitely-generated-cones)
      - [Conic combination](#conic-combination)
    - [Copositive cone](#copositive-cone)
      - [Duality of copositive and completely positive cones](#duality-of-copositive-and-completely-positive-cones)
      - [Interior of the copositive cone](#interior-of-the-copositive-cone)
      - [Positive-semidefinite-plus-nonnegative cone](#positive-semidefinite-plus-nonnegative-cone)
    - [Positive semidefinite cone](#positive-semidefinite-cone)
      - [Elliptope](#elliptope)
      - [Fantope](#fantope)
      - [Trace constraint](#trace-constraint)
        - [Positive semidefinite trace ball](#positive-semidefinite-trace-ball)
          - [Projection onto a positive semidefinite trace ball](#projection-onto-a-positive-semidefinite-trace-ball)
- [Game theory](game-theory.md)
  - [Prisoner's dilemma](game-theory.md#prisoner-s-dilemma)
    - [Iterated prisoner's dilemma](game-theory.md#iterated-prisoner-s-dilemma)
      - [Reactive strategy (game theory)](game-theory.md#reactive-strategy-game-theory)
        - [Always defect](game-theory.md#always-defect)
        - [Always cooperate](game-theory.md#always-cooperate)
        - [Tit for tat](game-theory.md#tit-for-tat)
          - [Tit for tat invasion of a reactive resident](game-theory.md#tit-for-tat-invasion-of-a-reactive-resident)
            - [Finite-horizon invasion threshold of Tit for tat against unconditional defection](game-theory.md#finite-horizon-invasion-threshold-of-tit-for-tat-against-unconditional-defection)
          - [Neutrality between Tit for tat and unconditional cooperation](game-theory.md#neutrality-between-tit-for-tat-and-unconditional-cooperation)
        - [Long-run payoff of reactive strategies](game-theory.md#long-run-payoff-of-reactive-strategies)
  - [Evolutionary game theory](game-theory.md#evolutionary-game-theory)
    - [Replicator equation](game-theory.md#replicator-equation)
  - [Repeated game](game-theory.md#repeated-game)
  - [Payoff](game-theory.md#payoff)
  - [Costly turnout game](game-theory.md#costly-turnout-game)
    - [Turnout equilibria with two supporters and one opponent](game-theory.md#turnout-equilibria-with-two-supporters-and-one-opponent)
    - [Pivotal voting probability](game-theory.md#pivotal-voting-probability)
  - [Nonatomic congestion game](game-theory.md#nonatomic-congestion-game)
  - [Congestion game](game-theory.md#congestion-game)
  - [Evolutionarily stable strategy](game-theory.md#evolutionarily-stable-strategy)
    - [Selection gradient](game-theory.md#selection-gradient)
    - [Hawk-Dove game](game-theory.md#hawk-dove-game)
    - [Two-condition criterion for evolutionary stability](game-theory.md#two-condition-criterion-for-evolutionary-stability)
  - [Security level payoff](game-theory.md#security-level-payoff)
  - [Nash bargaining problem](game-theory.md#nash-bargaining-problem)
    - [Negotiation set in two-person bargaining](game-theory.md#negotiation-set-in-two-person-bargaining)
    - [Joint dominance of payoff vectors](game-theory.md#joint-dominance-of-payoff-vectors)
    - [Bargaining individual rationality](game-theory.md#bargaining-individual-rationality)
    - [Bargaining independence of irrelevant alternatives](game-theory.md#bargaining-independence-of-irrelevant-alternatives)
    - [Positive affine invariance in bargaining](game-theory.md#positive-affine-invariance-in-bargaining)
    - [Bargaining symmetry](game-theory.md#bargaining-symmetry)
    - [Nash bargaining solution](game-theory.md#nash-bargaining-solution)
      - [Maximin bargaining solution](game-theory.md#maximin-bargaining-solution)
      - [Supporting triangle for Nash bargaining](game-theory.md#supporting-triangle-for-nash-bargaining)
      - [Nash product](game-theory.md#nash-product)
    - [Disagreement point](game-theory.md#disagreement-point)
  - [Cooperative game theory](game-theory.md#cooperative-game-theory)
    - [Transferable utility game](game-theory.md#transferable-utility-game)
      - [Coverage coalitional game](game-theory.md#coverage-coalitional-game)
        - [Shapley value of a coverage game](game-theory.md#shapley-value-of-a-coverage-game)
        - [Core of a coverage game](game-theory.md#core-of-a-coverage-game)
      - [Bankruptcy game](game-theory.md#bankruptcy-game)
      - [Superadditive coalitional game](game-theory.md#superadditive-coalitional-game)
      - [Glove game](game-theory.md#glove-game)
        - [Core of a glove game](game-theory.md#core-of-a-glove-game)
      - [Characteristic function of a coalitional game](game-theory.md#characteristic-function-of-a-coalitional-game)
      - [Dual coalitional game](game-theory.md#dual-coalitional-game)
      - [Nucleolus](game-theory.md#nucleolus)
        - [Prenucleolus](game-theory.md#prenucleolus)
      - [Imputation in a coalitional game](game-theory.md#imputation-in-a-coalitional-game)
      - [Marginal contribution](game-theory.md#marginal-contribution)
      - [Coalition (game theory)](game-theory.md#coalition-game-theory)
        - [Excess of a coalition](game-theory.md#excess-of-a-coalition)
      - [Convex cooperative game](game-theory.md#convex-cooperative-game)
        - [Shapley population monotonicity in a convex game](game-theory.md#shapley-population-monotonicity-in-a-convex-game)
        - [Shapley value belongs to the core of a convex game](game-theory.md#shapley-value-belongs-to-the-core-of-a-convex-game)
      - [Core (game theory)](game-theory.md#core-game-theory)
        - [Core of the miners game](game-theory.md#core-of-the-miners-game)
      - [Shapley value](game-theory.md#shapley-value)
        - [Shapley limit in a buyer-heavy exchange market](game-theory.md#shapley-limit-in-a-buyer-heavy-exchange-market)
        - [Balanced contributions of Shapley values](game-theory.md#balanced-contributions-of-shapley-values)
        - [Shapley wages in an entrepreneur-worker game](game-theory.md#shapley-wages-in-an-entrepreneur-worker-game)
        - [Shapley self-duality](game-theory.md#shapley-self-duality)
        - [Marginal contribution vector](game-theory.md#marginal-contribution-vector)
      - [Weighted voting game](game-theory.md#weighted-voting-game)
      - [Simple cooperative game](game-theory.md#simple-cooperative-game)
  - [Payoff-equivalent strategies](game-theory.md#payoff-equivalent-strategies)
  - [Normal-form game](game-theory.md#normal-form-game)
  - [Subgame perfect equilibrium](game-theory.md#subgame-perfect-equilibrium)
  - [Stackelberg competition](game-theory.md#stackelberg-competition)
    - [Stackelberg equilibrium](game-theory.md#stackelberg-equilibrium)
  - [Contest theory](game-theory.md#contest-theory)
    - [Sequential elimination all-pay contest](game-theory.md#sequential-elimination-all-pay-contest)
      - [Backward-induction threshold in an elimination all-pay contest](game-theory.md#backward-induction-threshold-in-an-elimination-all-pay-contest)
        - [Vanishing-discount limit of an elimination all-pay contest](game-theory.md#vanishing-discount-limit-of-an-elimination-all-pay-contest)
          - [Ranked winning probabilities in an undiscounted elimination contest](game-theory.md#ranked-winning-probabilities-in-an-undiscounted-elimination-contest)
      - [Discounted continuation value in an elimination contest](game-theory.md#discounted-continuation-value-in-an-elimination-contest)
        - [Effective prize in a sequential contest](game-theory.md#effective-prize-in-a-sequential-contest)
    - [Sequential private-value all-pay contest](game-theory.md#sequential-private-value-all-pay-contest)
      - [Ex ante follower advantage in a sequential all-pay contest](game-theory.md#ex-ante-follower-advantage-in-a-sequential-all-pay-contest)
      - [Leader optimization in a sequential private-value all-pay contest](game-theory.md#leader-optimization-in-a-sequential-private-value-all-pay-contest)
        - [Best-response selection at a flat leader objective](game-theory.md#best-response-selection-at-a-flat-leader-objective)
        - [Median-density threshold for the leader in an all-pay contest](game-theory.md#median-density-threshold-for-the-leader-in-an-all-pay-contest)
    - [Proportional allocation contest](game-theory.md#proportional-allocation-contest)
      - [Proportional contest with outside effort](game-theory.md#proportional-contest-with-outside-effort)
        - [Active-set threshold for a proportional contest with outside effort](game-theory.md#active-set-threshold-for-a-proportional-contest-with-outside-effort)
        - [Total-effort formula for a proportional contest with outside effort](game-theory.md#total-effort-formula-for-a-proportional-contest-with-outside-effort)
      - [Quadratic-cost two-player proportional contest](game-theory.md#quadratic-cost-two-player-proportional-contest)
    - [Simultaneous all-pay contests](game-theory.md#simultaneous-all-pay-contests)
      - [Two-of-three all-pay participation equilibrium](game-theory.md#two-of-three-all-pay-participation-equilibrium)
        - [Marginal-equivalent equilibria in additive contests](game-theory.md#marginal-equivalent-equilibria-in-additive-contests)
      - [All-pay indifference equation with random entry](game-theory.md#all-pay-indifference-equation-with-random-entry)
    - [Rank-order contest](game-theory.md#rank-order-contest)
      - [All-pay effort identity](game-theory.md#all-pay-effort-identity)
        - [Expected effort in a rank-order contest](game-theory.md#expected-effort-in-a-rank-order-contest)
          - [Uniform-value multi-prize all-pay effort formula](game-theory.md#uniform-value-multi-prize-all-pay-effort-formula)
            - [Discrete prize-count optimization for a power-valued contest](game-theory.md#discrete-prize-count-optimization-for-a-power-valued-contest)
      - [Rank-order expected prize allocation](game-theory.md#rank-order-expected-prize-allocation)
    - [Prize allocation rule](game-theory.md#prize-allocation-rule)
      - [Winning probability](game-theory.md#winning-probability)
  - [Bayesian game](game-theory.md#bayesian-game)
    - [Bayesian Nash equilibrium](game-theory.md#bayesian-nash-equilibrium)
  - [Mechanism design](game-theory.md#mechanism-design)
    - [Expected seller revenue](game-theory.md#expected-seller-revenue)
    - [Posted price](game-theory.md#posted-price)
    - [Mechanism (mechanism design)](game-theory.md#mechanism-mechanism-design)
    - [Single-parameter mechanism](game-theory.md#single-parameter-mechanism)
      - [Virtual valuation](game-theory.md#virtual-valuation)
        - [Virtual surplus](game-theory.md#virtual-surplus)
        - [Virtual-surplus revenue identity](game-theory.md#virtual-surplus-revenue-identity)
          - [Revenue-optimal public-project auction](game-theory.md#revenue-optimal-public-project-auction)
        - [Regular distribution (economics)](game-theory.md#regular-distribution-economics)
    - [Direct revelation mechanism](game-theory.md#direct-revelation-mechanism)
      - [Revelation principle](game-theory.md#revelation-principle)
      - [Vickrey-Clarke-Groves mechanism](game-theory.md#vickrey-clarke-groves-mechanism)
    - [Incentive compatibility](game-theory.md#incentive-compatibility)
      - [Dominant-strategy incentive compatibility](game-theory.md#dominant-strategy-incentive-compatibility)
        - [Critical-value payment](game-theory.md#critical-value-payment)
      - [Bayesian incentive compatibility](game-theory.md#bayesian-incentive-compatibility)
    - [Individual rationality](game-theory.md#individual-rationality)
      - [Ex post individual rationality](game-theory.md#ex-post-individual-rationality)
      - [Interim individual rationality](game-theory.md#interim-individual-rationality)
    - [Auction](game-theory.md#auction)
      - [Vickrey auction](game-theory.md#vickrey-auction)
      - [Lowest-price auction](game-theory.md#lowest-price-auction)
        - [Uniform lowest-price auction equilibrium](game-theory.md#uniform-lowest-price-auction-equilibrium)
      - [Reserve price](game-theory.md#reserve-price)
      - [English auction](game-theory.md#english-auction)
      - [Least unique bid auction](game-theory.md#least-unique-bid-auction)
        - [Two-bid three-player least unique bid auction](game-theory.md#two-bid-three-player-least-unique-bid-auction)
      - [All-pay auction](game-theory.md#all-pay-auction)
        - [Two-player complete-information all-pay equilibrium](game-theory.md#two-player-complete-information-all-pay-equilibrium)
      - [First-price sealed-bid auction](game-theory.md#first-price-sealed-bid-auction)
        - [No dominant positive-value bid in a first-price auction](game-theory.md#no-dominant-positive-value-bid-in-a-first-price-auction)
        - [Uniform private-value first-price bidding equilibrium](game-theory.md#uniform-private-value-first-price-bidding-equilibrium)
      - [Interim payment identity](game-theory.md#interim-payment-identity)
        - [Revenue equivalence](game-theory.md#revenue-equivalence)
      - [Private-value auction](game-theory.md#private-value-auction)
        - [Unit-demand valuation](game-theory.md#unit-demand-valuation)
        - [Independent private values model](game-theory.md#independent-private-values-model)
          - [Symmetric independent private values model](game-theory.md#symmetric-independent-private-values-model)
          - [Revenue comparison for two uniform private values](game-theory.md#revenue-comparison-for-two-uniform-private-values)
    - [Strategyproofness](game-theory.md#strategyproofness)
      - [Rank-raising monotonicity lemma](game-theory.md#rank-raising-monotonicity-lemma)
      - [Gibbard-Satterthwaite theorem](game-theory.md#gibbard-satterthwaite-theorem)
        - [Binary social ordering from strategyproof choice](game-theory.md#binary-social-ordering-from-strategyproof-choice)
          - [Two-voter dictatorship from binary choice](game-theory.md#two-voter-dictatorship-from-binary-choice)
        - [Top-bottom decisiveness lemma](game-theory.md#top-bottom-decisiveness-lemma)
    - [Social choice theory](game-theory.md#social-choice-theory)
      - [Condorcet winner](game-theory.md#condorcet-winner)
        - [Weak Condorcet winner](game-theory.md#weak-condorcet-winner)
      - [Single-peaked preferences](game-theory.md#single-peaked-preferences)
        - [Median voter rule](game-theory.md#median-voter-rule)
      - [Social choice function](game-theory.md#social-choice-function)
        - [Two-alternative majority rule](game-theory.md#two-alternative-majority-rule)
        - [Dictatorship in social choice](game-theory.md#dictatorship-in-social-choice)
          - [Dictator in social choice](game-theory.md#dictator-in-social-choice)
  - [Pure strategy](game-theory.md#pure-strategy)
    - [Strict dominance](game-theory.md#strict-dominance)
  - [Finite game](game-theory.md#finite-game)
    - [Symmetric finite game](game-theory.md#symmetric-finite-game)
  - [Mixed strategy](game-theory.md#mixed-strategy)
    - [Support of a mixed strategy](game-theory.md#support-of-a-mixed-strategy)
    - [Strategy support](game-theory.md#strategy-support)
  - [Bimatrix game](game-theory.md#bimatrix-game)
    - [Matching pennies](game-theory.md#matching-pennies)
    - [Lottery over joint action profiles](game-theory.md#lottery-over-joint-action-profiles)
    - [Support enumeration for a bimatrix game](game-theory.md#support-enumeration-for-a-bimatrix-game)
    - [Symmetric bimatrix game](game-theory.md#symmetric-bimatrix-game)
    - [Nondegeneracy of a bimatrix game](game-theory.md#nondegeneracy-of-a-bimatrix-game)
    - [Nash equilibrium](game-theory.md#nash-equilibrium)
      - [Ranked university application game](game-theory.md#ranked-university-application-game)
      - [Symmetric Nash equilibrium](game-theory.md#symmetric-nash-equilibrium)
      - [Equilibrium oddness theorem](game-theory.md#equilibrium-oddness-theorem)
      - [Symmetric equilibrium](game-theory.md#symmetric-equilibrium)
        - [Symmetric equilibrium parity](game-theory.md#symmetric-equilibrium-parity)
        - [Symmetric Nash gain map](game-theory.md#symmetric-nash-gain-map)
          - [Gain-map proof of symmetric equilibrium](game-theory.md#gain-map-proof-of-symmetric-equilibrium)
      - [Complementarity construction of a symmetric Nash equilibrium](game-theory.md#complementarity-construction-of-a-symmetric-nash-equilibrium)
      - [Lemke-Howson algorithm](game-theory.md#lemke-howson-algorithm)
        - [Complementary pivoting](game-theory.md#complementary-pivoting)
      - [Nash's theorem](game-theory.md#nash-s-theorem)
        - [Brouwer gain-map proof of bimatrix equilibrium](game-theory.md#brouwer-gain-map-proof-of-bimatrix-equilibrium)
      - [Brouwer proof of Nash equilibrium for a two-by-two game](game-theory.md#brouwer-proof-of-nash-equilibrium-for-a-two-by-two-game)
  - [Best response](game-theory.md#best-response)
    - [Dominant strategy](game-theory.md#dominant-strategy)
      - [Strictly dominant strategy](game-theory.md#strictly-dominant-strategy)
  - [Zero-sum game](game-theory.md#zero-sum-game)
    - [Rock paper scissors](game-theory.md#rock-paper-scissors)
    - [Value of a zero-sum game](game-theory.md#value-of-a-zero-sum-game)
    - [Cost-weighted finite search game](game-theory.md#cost-weighted-finite-search-game)
    - [Matrix game](game-theory.md#matrix-game)
      - [Positive-payoff linear programming for a matrix game](game-theory.md#positive-payoff-linear-programming-for-a-matrix-game)
      - [Payoff matrix](game-theory.md#payoff-matrix)
      - [Matrix-game optimization problem](game-theory.md#matrix-game-optimization-problem)
      - [Mixed-strategy optimality certificate for a matrix game](game-theory.md#mixed-strategy-optimality-certificate-for-a-matrix-game)
      - [Symmetric inverse formula for a matrix-game equilibrium](game-theory.md#symmetric-inverse-formula-for-a-matrix-game-equilibrium)
        - [Three-card threshold-sum zero-sum game](game-theory.md#three-card-threshold-sum-zero-sum-game)
    - [Minimax theorem](game-theory.md#minimax-theorem)
    - [Optimal mixed strategy](game-theory.md#optimal-mixed-strategy)
    - [Antisymmetric zero-sum game](game-theory.md#antisymmetric-zero-sum-game)
      - [Support certificate for an antisymmetric matrix game](game-theory.md#support-certificate-for-an-antisymmetric-matrix-game)
      - [Consecutive-number antisymmetric game](game-theory.md#consecutive-number-antisymmetric-game)
  - [Dominated strategy](game-theory.md#dominated-strategy)
    - [Dominated strategy elimination](game-theory.md#dominated-strategy-elimination)
    - [Weakly dominated strategy](game-theory.md#weakly-dominated-strategy)
      - [Equilibrium preservation under iterated weak dominance](game-theory.md#equilibrium-preservation-under-iterated-weak-dominance)
      - [Weak domination does not exclude equilibrium strategies](game-theory.md#weak-domination-does-not-exclude-equilibrium-strategies)
- [Mathematical finance](mathematical-finance.md)
  - [Financial return](mathematical-finance.md#financial-return)
  - [Financial market](mathematical-finance.md#financial-market)
  - [Financial asset](mathematical-finance.md#financial-asset)
    - [Credit derivative](mathematical-finance.md#credit-derivative)
      - [Synthetic CDO](mathematical-finance.md#synthetic-cdo)
        - [Credit tranche loss function](mathematical-finance.md#credit-tranche-loss-function)
      - [Credit-linked note](mathematical-finance.md#credit-linked-note)
      - [Total return swap](mathematical-finance.md#total-return-swap)
      - [Credit default swap](mathematical-finance.md#credit-default-swap)
        - [First-to-default swap](mathematical-finance.md#first-to-default-swap)
        - [Continuous-premium credit-default swap spread](mathematical-finance.md#continuous-premium-credit-default-swap-spread)
    - [Risk-free asset](mathematical-finance.md#risk-free-asset)
  - [Value at risk](mathematical-finance.md#value-at-risk)
    - [Compound-Poisson annual loss quantile](mathematical-finance.md#compound-poisson-annual-loss-quantile)
  - [Credit risk](mathematical-finance.md#credit-risk)
    - [Merton model](mathematical-finance.md#merton-model)
    - [Counterparty credit risk](mathematical-finance.md#counterparty-credit-risk)
    - [Credit spread](mathematical-finance.md#credit-spread)
      - [Credit spread option](mathematical-finance.md#credit-spread-option)
    - [Credit rating](mathematical-finance.md#credit-rating)
  - [Trinomial tree](mathematical-finance.md#trinomial-tree)
  - [Competitive equilibrium with one productive asset](mathematical-finance.md#competitive-equilibrium-with-one-productive-asset)
  - [Dominated martingale measure](mathematical-finance.md#dominated-martingale-measure)
  - [Relative-consumption share equilibrium](mathematical-finance.md#relative-consumption-share-equilibrium)
  - [Incomplete market](mathematical-finance.md#incomplete-market)
  - [Budget constraint](mathematical-finance.md#budget-constraint)
    - [Discrete dividend budget equation](mathematical-finance.md#discrete-dividend-budget-equation)
  - [Arithmetic stock model with constant volatility](mathematical-finance.md#arithmetic-stock-model-with-constant-volatility)
    - [Call price in an arithmetic stock model with interest](mathematical-finance.md#call-price-in-an-arithmetic-stock-model-with-interest)
      - [Delta bound in an arithmetic stock model](mathematical-finance.md#delta-bound-in-an-arithmetic-stock-model)
  - [Local volatility](mathematical-finance.md#local-volatility)
    - [Local volatility model](mathematical-finance.md#local-volatility-model)
      - [Exponential claim in a driftless square-root model](mathematical-finance.md#exponential-claim-in-a-driftless-square-root-model)
      - [Pricing equation for a local volatility model](mathematical-finance.md#pricing-equation-for-a-local-volatility-model)
        - [Explicit log-price scheme for local-volatility pricing](mathematical-finance.md#explicit-log-price-scheme-for-local-volatility-pricing)
          - [Finite-difference option Greeks](mathematical-finance.md#finite-difference-option-greeks)
        - [Delta replication from a local-volatility pricing equation](mathematical-finance.md#delta-replication-from-a-local-volatility-pricing-equation)
      - [Dupire equation](mathematical-finance.md#dupire-equation)
        - [Local volatility recovery from call prices](mathematical-finance.md#local-volatility-recovery-from-call-prices)
      - [Brownian representation replication in a local volatility market](mathematical-finance.md#brownian-representation-replication-in-a-local-volatility-market)
  - [Credit default](mathematical-finance.md#credit-default)
    - [Loss given default](mathematical-finance.md#loss-given-default)
    - [Default time](mathematical-finance.md#default-time)
      - [Default intensity](mathematical-finance.md#default-intensity)
  - [Investment portfolio](mathematical-finance.md#investment-portfolio)
    - [Portfolio diversification](mathematical-finance.md#portfolio-diversification)
    - [Short (finance)](mathematical-finance.md#short-finance)
    - [Expected return](mathematical-finance.md#expected-return)
    - [Portfolio wealth](mathematical-finance.md#portfolio-wealth)
    - [Brownian portfolio exposures](mathematical-finance.md#brownian-portfolio-exposures)
    - [Sharpe ratio](mathematical-finance.md#sharpe-ratio)
    - [Market portfolio](mathematical-finance.md#market-portfolio)
      - [Sign of the normalized tangency portfolio](mathematical-finance.md#sign-of-the-normalized-tangency-portfolio)
      - [Capital market line](mathematical-finance.md#capital-market-line)
      - [Capital asset pricing model](mathematical-finance.md#capital-asset-pricing-model)
      - [Beta of an asset](mathematical-finance.md#beta-of-an-asset)
  - [Stock](mathematical-finance.md#stock)
    - [Continuous dividend yield](mathematical-finance.md#continuous-dividend-yield)
    - [Geometric stock index](mathematical-finance.md#geometric-stock-index)
    - [Defaultable stock](mathematical-finance.md#defaultable-stock)
      - [Zero-recovery default model](mathematical-finance.md#zero-recovery-default-model)
  - [Numéraire](mathematical-finance.md#numeraire)
    - [Change of numeraire](mathematical-finance.md#change-of-numeraire)
      - [Stock-numeraire measure in the Black-Scholes model](mathematical-finance.md#stock-numeraire-measure-in-the-black-scholes-model)
    - [Numéraire portfolio](mathematical-finance.md#numeraire-portfolio)
      - [Numéraire strategy](mathematical-finance.md#numeraire-strategy)
  - [Arbitrage](mathematical-finance.md#arbitrage)
    - [Arbitrage pricing theory](mathematical-finance.md#arbitrage-pricing-theory)
      - [Covariance criterion for diversification of factor residuals](mathematical-finance.md#covariance-criterion-for-diversification-of-factor-residuals)
      - [Exact factor pricing without a traded risk-free asset](mathematical-finance.md#exact-factor-pricing-without-a-traded-risk-free-asset)
      - [Exact factor pricing without idiosyncratic risk](mathematical-finance.md#exact-factor-pricing-without-idiosyncratic-risk)
    - [Singular-volatility drift arbitrage](mathematical-finance.md#singular-volatility-drift-arbitrage)
    - [Law of one price](mathematical-finance.md#law-of-one-price)
      - [Strict local martingale failure of the law of one price](mathematical-finance.md#strict-local-martingale-failure-of-the-law-of-one-price)
    - [Investment-consumption arbitrage](mathematical-finance.md#investment-consumption-arbitrage)
      - [Pure-investment arbitrage](mathematical-finance.md#pure-investment-arbitrage)
      - [Consumption](mathematical-finance.md#consumption)
      - [Terminal-consumption arbitrage](mathematical-finance.md#terminal-consumption-arbitrage)
    - [Arbitrage in a one-period Gaussian market](mathematical-finance.md#arbitrage-in-a-one-period-gaussian-market)
    - [Self-financing portfolio](mathematical-finance.md#self-financing-portfolio)
      - [Portfolio with constant stock value in bond units](mathematical-finance.md#portfolio-with-constant-stock-value-in-bond-units)
      - [Constant-proportion portfolio](mathematical-finance.md#constant-proportion-portfolio)
      - [Self-financing conditions for smooth stock and bond holdings](mathematical-finance.md#self-financing-conditions-for-smooth-stock-and-bond-holdings)
      - [Discounted dividend gains](mathematical-finance.md#discounted-dividend-gains)
        - [Multi-period dividend pricing identity](mathematical-finance.md#multi-period-dividend-pricing-identity)
        - [Dividend-inclusive portfolio return](mathematical-finance.md#dividend-inclusive-portfolio-return)
      - [Admissible trading strategy](mathematical-finance.md#admissible-trading-strategy)
      - [Discounted wealth equation in discrete time](mathematical-finance.md#discounted-wealth-equation-in-discrete-time)
        - [Discounted wealth martingale integrability condition](mathematical-finance.md#discounted-wealth-martingale-integrability-condition)
  - [Utility function](utility-function.md)
    - [Risk seeking](utility-function.md#risk-seeking)
    - [Risk aversion](utility-function.md#risk-aversion)
      - [Relative risk aversion coefficient](utility-function.md#relative-risk-aversion-coefficient)
        - [Small multiplicative risk premium](utility-function.md#small-multiplicative-risk-premium)
    - [Marginal utility](utility-function.md#marginal-utility)
    - [Expected utility](utility-function.md#expected-utility)
      - [Risk premium](utility-function.md#risk-premium)
    - [Affine utility on probability measures](utility-function.md#affine-utility-on-probability-measures)
      - [Expected utility representation on a finite measurable space](utility-function.md#expected-utility-representation-on-a-finite-measurable-space)
      - [Positive affine uniqueness of affine preference representations](utility-function.md#positive-affine-uniqueness-of-affine-preference-representations)
      - [Mixture solvability of affine preferences](utility-function.md#mixture-solvability-of-affine-preferences)
      - [Independence axiom for lottery preferences](utility-function.md#independence-axiom-for-lottery-preferences)
    - [Inverse marginal utility](utility-function.md#inverse-marginal-utility)
    - [Multiplicative habit utility](utility-function.md#multiplicative-habit-utility)
      - [Dual equation for multiplicative habit investment](utility-function.md#dual-equation-for-multiplicative-habit-investment)
      - [Effective consumption shadow price with habit](utility-function.md#effective-consumption-shadow-price-with-habit)
      - [Exponentially weighted consumption habit](utility-function.md#exponentially-weighted-consumption-habit)
    - [Inada conditions](utility-function.md#inada-conditions)
      - [Inada utility with vanishing curvature](utility-function.md#inada-utility-with-vanishing-curvature)
    - [Constant relative risk aversion utility](utility-function.md#constant-relative-risk-aversion-utility)
      - [Power-wealth investment with running utility](utility-function.md#power-wealth-investment-with-running-utility)
      - [Benchmark-relative power-utility portfolio](utility-function.md#benchmark-relative-power-utility-portfolio)
      - [Square-root investment-consumption value](utility-function.md#square-root-investment-consumption-value)
      - [Logarithmic utility](utility-function.md#logarithmic-utility)
        - [Two-state logarithmic portfolio with a borrowing constraint](utility-function.md#two-state-logarithmic-portfolio-with-a-borrowing-constraint)
        - [Log-optimal investment with Gaussian drift learning](utility-function.md#log-optimal-investment-with-gaussian-drift-learning)
      - [Volatility-penalized terminal fee](utility-function.md#volatility-penalized-terminal-fee)
      - [Risk aversion recovered from an optimal two-state payoff](utility-function.md#risk-aversion-recovered-from-an-optimal-two-state-payoff)
    - [Quasilinear utility](utility-function.md#quasilinear-utility)
    - [Risk neutrality](utility-function.md#risk-neutrality)
    - [Constant absolute risk aversion utility](utility-function.md#constant-absolute-risk-aversion-utility)
      - [Binomial exponential-utility terminal wealth](utility-function.md#binomial-exponential-utility-terminal-wealth)
      - [Finite-horizon exponential-utility portfolio](utility-function.md#finite-horizon-exponential-utility-portfolio)
      - [Exponential-utility risk sharing](utility-function.md#exponential-utility-risk-sharing)
      - [Exponential-utility portfolio with nonnegative cash](utility-function.md#exponential-utility-portfolio-with-nonnegative-cash)
    - [Expected utility hypothesis](utility-function.md#expected-utility-hypothesis)
      - [Expected utility maximization](utility-function.md#expected-utility-maximization)
        - [Unbounded linear terminal-wealth utility](utility-function.md#unbounded-linear-terminal-wealth-utility)
        - [Complete-market terminal utility optimizer](utility-function.md#complete-market-terminal-utility-optimizer)
          - [Binomial power-utility terminal wealth](utility-function.md#binomial-power-utility-terminal-wealth)
        - [Proportional transaction cost](utility-function.md#proportional-transaction-cost)
        - [Secant domination for expected utility derivatives](utility-function.md#secant-domination-for-expected-utility-derivatives)
        - [Terminal wealth floor](utility-function.md#terminal-wealth-floor)
          - [Floored marginal utility optimizer](utility-function.md#floored-marginal-utility-optimizer)
        - [Discounted infinite-horizon utility integrability](utility-function.md#discounted-infinite-horizon-utility-integrability)
        - [Hedge fund incentive utility](utility-function.md#hedge-fund-incentive-utility)
          - [Concavification of incentive utility](utility-function.md#concavification-of-incentive-utility)
            - [Fair-game gambling induced by an incentive fee](utility-function.md#fair-game-gambling-induced-by-an-incentive-fee)
            - [Common tangent for exponential incentive utility](utility-function.md#common-tangent-for-exponential-incentive-utility)
        - [Investment-consumption problem](utility-function.md#investment-consumption-problem)
          - [Finite-horizon power-utility investment and consumption](utility-function.md#finite-horizon-power-utility-investment-and-consumption)
          - [Finite-horizon logarithmic investment and consumption](utility-function.md#finite-horizon-logarithmic-investment-and-consumption)
          - [Investment with fixed debt service](utility-function.md#investment-with-fixed-debt-service)
            - [Dual ruin boundary with debt service](utility-function.md#dual-ruin-boundary-with-debt-service)
          - [Constant market price of risk investment](utility-function.md#constant-market-price-of-risk-investment)
          - [Consumption satisfaction stock](utility-function.md#consumption-satisfaction-stock)
            - [Singular consumption control](utility-function.md#singular-consumption-control)
            - [Gradient constraint for unbounded consumption](utility-function.md#gradient-constraint-for-unbounded-consumption)
            - [Wealth-to-satisfaction reduction](utility-function.md#wealth-to-satisfaction-reduction)
          - [Investment value transversality condition](utility-function.md#investment-value-transversality-condition)
          - [State-dependent correlation investment problem](utility-function.md#state-dependent-correlation-investment-problem)
            - [Power transformation of a complete-market investment equation](utility-function.md#power-transformation-of-a-complete-market-investment-equation)
          - [Intertemporal hedging demand](utility-function.md#intertemporal-hedging-demand)
            - [Learning hedge in a binary-drift investment model](utility-function.md#learning-hedge-in-a-binary-drift-investment-model)
          - [High-water mark investment taxation](utility-function.md#high-water-mark-investment-taxation)
            - [Wealth-cap investment boundary](utility-function.md#wealth-cap-investment-boundary)
            - [High-water mark tax boundary condition](utility-function.md#high-water-mark-tax-boundary-condition)
          - [Merton consumption-investment problem](utility-function.md#merton-consumption-investment-problem)
            - [Regime-switching Merton equations](utility-function.md#regime-switching-merton-equations)
            - [Retirement boundary with an income option](utility-function.md#retirement-boundary-with-an-income-option)
            - [Merton consumption constant](utility-function.md#merton-consumption-constant)
            - [Maximal squared Sharpe ratio value bound](utility-function.md#maximal-squared-sharpe-ratio-value-bound)
            - [Exponential interest-rate switch](utility-function.md#exponential-interest-rate-switch)
        - [Certainty equivalent](utility-function.md#certainty-equivalent)
        - [Expected utility of a Gaussian location-scale family](utility-function.md#expected-utility-of-a-gaussian-location-scale-family)
        - [Indifference price](utility-function.md#indifference-price)
          - [Periodic utility indifference payment for Gaussian income](utility-function.md#periodic-utility-indifference-payment-for-gaussian-income)
        - [Optimized affine shift of concave utility](utility-function.md#optimized-affine-shift-of-concave-utility)
        - [Scaled centered risk under concave utility](utility-function.md#scaled-centered-risk-under-concave-utility)
        - [Utility duality with martingale deflators](utility-function.md#utility-duality-with-martingale-deflators)
          - [Logarithmic terminal wealth in a complete market](utility-function.md#logarithmic-terminal-wealth-in-a-complete-market)
          - [Optimal marginal utility as a one-period pricing density](utility-function.md#optimal-marginal-utility-as-a-one-period-pricing-density)
            - [Marginal utility price](utility-function.md#marginal-utility-price)
            - [Marginal utility pricing with proportional transaction costs](utility-function.md#marginal-utility-pricing-with-proportional-transaction-costs)
          - [One-period marginal-utility certificate of optimality](utility-function.md#one-period-marginal-utility-certificate-of-optimality)
          - [Marginal-utility verification of optimal consumption](utility-function.md#marginal-utility-verification-of-optimal-consumption)
          - [Wealth-variable Legendre dual](utility-function.md#wealth-variable-legendre-dual)
  - [Discrete-time expected-utility portfolio problem](mathematical-finance.md#discrete-time-expected-utility-portfolio-problem)
    - [Exponential-utility trading with Gaussian increments](mathematical-finance.md#exponential-utility-trading-with-gaussian-increments)
      - [Hedging a Gaussian income stream with exponential utility](mathematical-finance.md#hedging-a-gaussian-income-stream-with-exponential-utility)
    - [Bellman equation for terminal-wealth utility](mathematical-finance.md#bellman-equation-for-terminal-wealth-utility)
      - [Monotonicity and concavity of a portfolio value function](mathematical-finance.md#monotonicity-and-concavity-of-a-portfolio-value-function)
  - [Risk-neutral measure](mathematical-finance.md#risk-neutral-measure)
    - [Risk-neutral probability](mathematical-finance.md#risk-neutral-probability)
    - [Martingale characterization by bounded self-financing strategies](mathematical-finance.md#martingale-characterization-by-bounded-self-financing-strategies)
    - [Risk-neutral pricing](mathematical-finance.md#risk-neutral-pricing)
    - [Martingale deflator](mathematical-finance.md#martingale-deflator)
      - [Bounded-coefficient asset deflator](mathematical-finance.md#bounded-coefficient-asset-deflator)
      - [Positive regression deflator in a complete finite market](mathematical-finance.md#positive-regression-deflator-in-a-complete-finite-market)
      - [Local martingale deflator](mathematical-finance.md#local-martingale-deflator)
        - [Zero-capital nonnegative wealth under a local deflator](mathematical-finance.md#zero-capital-nonnegative-wealth-under-a-local-deflator)
        - [Deflator-based claim replication](mathematical-finance.md#deflator-based-claim-replication)
          - [Dollar portfolio from a deflated wealth martingale](mathematical-finance.md#dollar-portfolio-from-a-deflated-wealth-martingale)
        - [Market price of risk](mathematical-finance.md#market-price-of-risk)
          - [Short-rate market price of risk](mathematical-finance.md#short-rate-market-price-of-risk)
          - [Singular initial market-price-of-risk obstruction](mathematical-finance.md#singular-initial-market-price-of-risk-obstruction)
      - [State-price density](mathematical-finance.md#state-price-density)
        - [Marginal utility pricing in a dividend economy](mathematical-finance.md#marginal-utility-pricing-in-a-dividend-economy)
          - [Dividend-price transversality condition](mathematical-finance.md#dividend-price-transversality-condition)
            - [Transversality and fundamental dividend prices](mathematical-finance.md#transversality-and-fundamental-dividend-prices)
        - [Quadratic Ornstein-Uhlenbeck state-price density](mathematical-finance.md#quadratic-ornstein-uhlenbeck-state-price-density)
        - [Arrow–Debreu state price](mathematical-finance.md#arrow-debreu-state-price)
          - [Nonnegative state prices need not exclude arbitrage](mathematical-finance.md#nonnegative-state-prices-need-not-exclude-arbitrage)
        - [State-price density and local deflator distinction](mathematical-finance.md#state-price-density-and-local-deflator-distinction)
        - [Deflated wealth equation with consumption](mathematical-finance.md#deflated-wealth-equation-with-consumption)
          - [Supermartingale control of deflated consumption gains](mathematical-finance.md#supermartingale-control-of-deflated-consumption-gains)
        - [State-price budget constraint](mathematical-finance.md#state-price-budget-constraint)
          - [Hölder bound for discounted CRRA consumption](mathematical-finance.md#holder-bound-for-discounted-crra-consumption)
        - [Exponential minimization construction of a bounded pricing kernel](mathematical-finance.md#exponential-minimization-construction-of-a-bounded-pricing-kernel)
      - [One-period martingale deflator](mathematical-finance.md#one-period-martingale-deflator)
    - [Forward measure](mathematical-finance.md#forward-measure)
      - [T-forward measure](mathematical-finance.md#t-forward-measure)
    - [Equivalent local martingale measure](mathematical-finance.md#equivalent-local-martingale-measure)
      - [Equivalent local martingale measures exclude admissible arbitrage](mathematical-finance.md#equivalent-local-martingale-measures-exclude-admissible-arbitrage)
  - [Binomial options pricing model](mathematical-finance.md#binomial-options-pricing-model)
    - [Discrete-time binomial market](mathematical-finance.md#discrete-time-binomial-market)
      - [Binomial-market probability density](mathematical-finance.md#binomial-market-probability-density)
      - [Risk-neutral probability in a binomial market](mathematical-finance.md#risk-neutral-probability-in-a-binomial-market)
      - [Replicating portfolio in a binomial market](mathematical-finance.md#replicating-portfolio-in-a-binomial-market)
        - [Convex-payoff delta monotonicity in a binomial market](mathematical-finance.md#convex-payoff-delta-monotonicity-in-a-binomial-market)
        - [Backward option pricing](mathematical-finance.md#backward-option-pricing)
      - [Stock-numeraire measure in a binomial market](mathematical-finance.md#stock-numeraire-measure-in-a-binomial-market)
  - [Fixed-income security](mathematical-finance.md#fixed-income-security)
    - [Zero-coupon bond](mathematical-finance.md#zero-coupon-bond)
      - [Zero-coupon yield to maturity](mathematical-finance.md#zero-coupon-yield-to-maturity)
      - [Floating-rate payment bond replication](mathematical-finance.md#floating-rate-payment-bond-replication)
      - [Linear bond pricing in a bounded short-rate diffusion](mathematical-finance.md#linear-bond-pricing-in-a-bounded-short-rate-diffusion)
        - [Forward-measure terminal rate in a linear bond model](mathematical-finance.md#forward-measure-terminal-rate-in-a-linear-bond-model)
      - [Exponential-affine bond pricing](mathematical-finance.md#exponential-affine-bond-pricing)
        - [Deterministic calibration of an autoregressive short rate](mathematical-finance.md#deterministic-calibration-of-an-autoregressive-short-rate)
    - [Interest rate](mathematical-finance.md#interest-rate)
      - [Interest-rate cap](mathematical-finance.md#interest-rate-cap)
        - [Caplet](mathematical-finance.md#caplet)
          - [Gaussian caplet bond-put formula](mathematical-finance.md#gaussian-caplet-bond-put-formula)
      - [Yield curve](mathematical-finance.md#yield-curve)
      - [Interest rate swap](mathematical-finance.md#interest-rate-swap)
        - [Par swap rate](mathematical-finance.md#par-swap-rate)
      - [Heath-Jarrow-Morton model](mathematical-finance.md#heath-jarrow-morton-model)
        - [Diagonal short-rate dynamics in the Heath-Jarrow-Morton model](mathematical-finance.md#diagonal-short-rate-dynamics-in-the-heath-jarrow-morton-model)
        - [One Brownian factor does not imply a Markov short rate](mathematical-finance.md#one-brownian-factor-does-not-imply-a-markov-short-rate)
        - [Gaussian forward-rate field](mathematical-finance.md#gaussian-forward-rate-field)
          - [Integrated Gaussian forward-rate process](mathematical-finance.md#integrated-gaussian-forward-rate-process)
            - [Gaussian forward-rate covariance drift restriction](mathematical-finance.md#gaussian-forward-rate-covariance-drift-restriction)
          - [Musiela forward-curve equation](mathematical-finance.md#musiela-forward-curve-equation)
            - [Stationary Gaussian forward curve](mathematical-finance.md#stationary-gaussian-forward-curve)
          - [Gaussian bond-option formula](mathematical-finance.md#gaussian-bond-option-formula)
        - [Forward-rate equation for a Markov short-rate diffusion](mathematical-finance.md#forward-rate-equation-for-a-markov-short-rate-diffusion)
        - [Discounted bond price martingale](mathematical-finance.md#discounted-bond-price-martingale)
      - [Discount factor](mathematical-finance.md#discount-factor)
      - [Instantaneous forward rate](mathematical-finance.md#instantaneous-forward-rate)
      - [Short rate](mathematical-finance.md#short-rate)
        - [Hull-White model](mathematical-finance.md#hull-white-model)
          - [Exact forward-curve fit in the Hull-White model](mathematical-finance.md#exact-forward-curve-fit-in-the-hull-white-model)
        - [One-factor short-rate model](mathematical-finance.md#one-factor-short-rate-model)
          - [Cox-Ross short-rate pricing equation](mathematical-finance.md#cox-ross-short-rate-pricing-equation)
          - [Instantaneous covariance rank in a one-factor rate model](mathematical-finance.md#instantaneous-covariance-rank-in-a-one-factor-rate-model)
          - [Short-rate bond pricing equation](mathematical-finance.md#short-rate-bond-pricing-equation)
            - [Short-rate diffusion hedging](mathematical-finance.md#short-rate-diffusion-hedging)
            - [Affine diffusion bond pricing](mathematical-finance.md#affine-diffusion-bond-pricing)
        - [Vasicek model](mathematical-finance.md#vasicek-model)
        - [Gaussian short-rate model with a deterministic shift](mathematical-finance.md#gaussian-short-rate-model-with-a-deterministic-shift)
          - [Forward-curve calibration of a shifted Brownian short rate](mathematical-finance.md#forward-curve-calibration-of-a-shifted-brownian-short-rate)
        - [Gaussian short-rate model with constant coefficients](mathematical-finance.md#gaussian-short-rate-model-with-constant-coefficients)
        - [Cox–Ingersoll–Ross model](mathematical-finance.md#cox-ingersoll-ross-model)
          - [Square root of a CIR diffusion](mathematical-finance.md#square-root-of-a-cir-diffusion)
          - [CIR bond pricing](mathematical-finance.md#cir-bond-pricing)
          - [Feller positivity condition for the CIR model](mathematical-finance.md#feller-positivity-condition-for-the-cir-model)
      - [Spot interest rate](mathematical-finance.md#spot-interest-rate)
      - [Bank account](mathematical-finance.md#bank-account)
        - [Rolling one-period bond account](mathematical-finance.md#rolling-one-period-bond-account)
        - [Continuous-time bank account](mathematical-finance.md#continuous-time-bank-account)
  - [Fundamental theorem of asset pricing](mathematical-finance.md#fundamental-theorem-of-asset-pricing)
    - [Positive-density separation proof of the one-period asset-pricing theorem](mathematical-finance.md#positive-density-separation-proof-of-the-one-period-asset-pricing-theorem)
    - [Gaussian-damped martingale density construction](mathematical-finance.md#gaussian-damped-martingale-density-construction)
    - [Positive state-price density alternative](mathematical-finance.md#positive-state-price-density-alternative)
    - [Complete market](mathematical-finance.md#complete-market)
      - [Completeness and uniqueness of dominated martingale measures](mathematical-finance.md#completeness-and-uniqueness-of-dominated-martingale-measures)
      - [Complete markets have unique state-price densities](mathematical-finance.md#complete-markets-have-unique-state-price-densities)
      - [Complete two-state market](mathematical-finance.md#complete-two-state-market)
      - [Uniqueness of a one-period pricing density](mathematical-finance.md#uniqueness-of-a-one-period-pricing-density)
      - [Finite branching bound in a complete market](mathematical-finance.md#finite-branching-bound-in-a-complete-market)
    - [Finite-state superhedging alternative](mathematical-finance.md#finite-state-superhedging-alternative)
    - [European call option](mathematical-finance.md#european-call-option)
      - [Down-and-out European call](mathematical-finance.md#down-and-out-european-call)
        - [Zero-rate barrier-strike call hedge](mathematical-finance.md#zero-rate-barrier-strike-call-hedge)
      - [Convexity of a European call price in strike](mathematical-finance.md#convexity-of-a-european-call-price-in-strike)
      - [Maturity monotonicity of calls with nonnegative strikes](mathematical-finance.md#maturity-monotonicity-of-calls-with-nonnegative-strikes)
      - [Power payoff static call representation](mathematical-finance.md#power-payoff-static-call-representation)
        - [Sharp power-call inequality](mathematical-finance.md#sharp-power-call-inequality)
        - [Call-price decay and moment threshold](mathematical-finance.md#call-price-decay-and-moment-threshold)
      - [Call-price density recovery](mathematical-finance.md#call-price-density-recovery)
        - [Finite-strike nonidentification of a pricing density](mathematical-finance.md#finite-strike-nonidentification-of-a-pricing-density)
        - [Power call-curve pricing density](mathematical-finance.md#power-call-curve-pricing-density)
      - [Butterfly-spread arbitrage for nonconvex call prices](mathematical-finance.md#butterfly-spread-arbitrage-for-nonconvex-call-prices)
      - [Vertical-spread arbitrage for increasing call prices](mathematical-finance.md#vertical-spread-arbitrage-for-increasing-call-prices)
      - [One-period call price bounds](mathematical-finance.md#one-period-call-price-bounds)
      - [Contour inversion for call prices](mathematical-finance.md#contour-inversion-for-call-prices)
      - [Discrete Dupire equation](mathematical-finance.md#discrete-dupire-equation)
      - [Discrete call-price curvature](mathematical-finance.md#discrete-call-price-curvature)
      - [Monotonicity of a European call price in strike](mathematical-finance.md#monotonicity-of-a-european-call-price-in-strike)
      - [Static replication on a finite terminal support](mathematical-finance.md#static-replication-on-a-finite-terminal-support)
        - [Discrete realized-variance replication identity](mathematical-finance.md#discrete-realized-variance-replication-identity)
      - [Put-call parity](mathematical-finance.md#put-call-parity)
        - [Power put-call parity](mathematical-finance.md#power-put-call-parity)
        - [Put-call symmetry in the Black-Scholes model](mathematical-finance.md#put-call-symmetry-in-the-black-scholes-model)
      - [Binomial call-price recursion](mathematical-finance.md#binomial-call-price-recursion)
      - [Forward-start call option](mathematical-finance.md#forward-start-call-option)
    - [Contingent claim](mathematical-finance.md#contingent-claim)
      - [Contingent claim payoff](mathematical-finance.md#contingent-claim-payoff)
      - [Path-dependent contingent claim](mathematical-finance.md#path-dependent-contingent-claim)
        - [Lookback option](mathematical-finance.md#lookback-option)
          - [Running-maximum boundary for a lookback option](mathematical-finance.md#running-maximum-boundary-for-a-lookback-option)
      - [Put option](mathematical-finance.md#put-option)
        - [European put option](mathematical-finance.md#european-put-option)
        - [American put option](mathematical-finance.md#american-put-option)
          - [Perpetual put option](mathematical-finance.md#perpetual-put-option)
            - [Dividend-yield sensitivity of the perpetual put trigger](mathematical-finance.md#dividend-yield-sensitivity-of-the-perpetual-put-trigger)
      - [Barrier option](mathematical-finance.md#barrier-option)
        - [Up-and-in claim](mathematical-finance.md#up-and-in-claim)
          - [Reflected European payoff for an up-and-in option](mathematical-finance.md#reflected-european-payoff-for-an-up-and-in-option)
        - [Up-and-out power claim](mathematical-finance.md#up-and-out-power-claim)
        - [Down-and-out claim](mathematical-finance.md#down-and-out-claim)
        - [Down-and-in claim](mathematical-finance.md#down-and-in-claim)
          - [Delta jump at activation of a down-and-in call](mathematical-finance.md#delta-jump-at-activation-of-a-down-and-in-call)
          - [Static terminal-payoff representation of a down-and-in claim](mathematical-finance.md#static-terminal-payoff-representation-of-a-down-and-in-claim)
      - [One-touch option](mathematical-finance.md#one-touch-option)
      - [Forward contract](mathematical-finance.md#forward-contract)
      - [Futures contract](mathematical-finance.md#futures-contract)
        - [Futures pricing](mathematical-finance.md#futures-pricing)
          - [Backwardation](mathematical-finance.md#backwardation)
          - [Contango](mathematical-finance.md#contango)
      - [Square-root stock claim](mathematical-finance.md#square-root-stock-claim)
        - [Square-root stock implied volatility](mathematical-finance.md#square-root-stock-implied-volatility)
          - [Half-volatility measure for a square-root stock claim](mathematical-finance.md#half-volatility-measure-for-a-square-root-stock-claim)
        - [Forward drift restriction for square-root stock claims](mathematical-finance.md#forward-drift-restriction-for-square-root-stock-claims)
        - [Conditional square-root price under independent volatility](mathematical-finance.md#conditional-square-root-price-under-independent-volatility)
      - [Claim replication](mathematical-finance.md#claim-replication)
        - [One-period quadratic hedge](mathematical-finance.md#one-period-quadratic-hedge)
          - [Fixed-capital quadratic hedge in a one-period market](mathematical-finance.md#fixed-capital-quadratic-hedge-in-a-one-period-market)
          - [Minimal martingale measure in a one-period market](mathematical-finance.md#minimal-martingale-measure-in-a-one-period-market)
            - [Negative minimal density in an arbitrage-free one-period market](mathematical-finance.md#negative-minimal-density-in-an-arbitrage-free-one-period-market)
          - [Signed martingale measure](mathematical-finance.md#signed-martingale-measure)
          - [Gaussian quadratic hedge](mathematical-finance.md#gaussian-quadratic-hedge)
          - [Minimum-norm one-period pricing weight](mathematical-finance.md#minimum-norm-one-period-pricing-weight)
        - [One-period Gram-matrix replication formula](mathematical-finance.md#one-period-gram-matrix-replication-formula)
        - [Telescoping replication of a stock-price sum](mathematical-finance.md#telescoping-replication-of-a-stock-price-sum)
        - [Superhedging](mathematical-finance.md#superhedging)
          - [Superhedging price](mathematical-finance.md#superhedging-price)
      - [Replicating strategy](mathematical-finance.md#replicating-strategy)
      - [European contingent claim](mathematical-finance.md#european-contingent-claim)
        - [Attainable European contingent claim](mathematical-finance.md#attainable-european-contingent-claim)
        - [Asian option](mathematical-finance.md#asian-option)
          - [Geometric Asian option](mathematical-finance.md#geometric-asian-option)
            - [Conditional geometric-average Asian option formula](mathematical-finance.md#conditional-geometric-average-asian-option-formula)
            - [Discrete geometric average under the stock-numeraire measure](mathematical-finance.md#discrete-geometric-average-under-the-stock-numeraire-measure)
              - [Stock-delivery option with a geometric average](mathematical-finance.md#stock-delivery-option-with-a-geometric-average)
        - [Chooser option](mathematical-finance.md#chooser-option)
        - [Power option](mathematical-finance.md#power-option)
        - [Binary option](mathematical-finance.md#binary-option)
          - [Barrier digital call](mathematical-finance.md#barrier-digital-call)
          - [Barrier digital put](mathematical-finance.md#barrier-digital-put)
          - [Digital call option](mathematical-finance.md#digital-call-option)
            - [Cash-at-hit digital call](mathematical-finance.md#cash-at-hit-digital-call)
          - [Digital put option](mathematical-finance.md#digital-put-option)
  - [Stochastic volatility model](mathematical-finance.md#stochastic-volatility-model)
    - [Exponential payoff transform PDE](mathematical-finance.md#exponential-payoff-transform-pde)
      - [Gaussian volatility exponential-quadratic transform](mathematical-finance.md#gaussian-volatility-exponential-quadratic-transform)
        - [Riccati moment-explosion horizon](mathematical-finance.md#riccati-moment-explosion-horizon)
    - [Spot volatility](mathematical-finance.md#spot-volatility)
    - [Heston model](mathematical-finance.md#heston-model)
  - [Black-Scholes model](mathematical-finance.md#black-scholes-model)
    - [Black-Scholes parameter sensitivities](mathematical-finance.md#black-scholes-parameter-sensitivities)
      - [Convexity preservation in Black-Scholes pricing](mathematical-finance.md#convexity-preservation-in-black-scholes-pricing)
      - [Option rho](mathematical-finance.md#option-rho)
      - [Option gamma](mathematical-finance.md#option-gamma)
    - [Random constant Gaussian interest-rate mixture](mathematical-finance.md#random-constant-gaussian-interest-rate-mixture)
    - [Logarithmic stock payoff](mathematical-finance.md#logarithmic-stock-payoff)
    - [Guaranteed terminal stock floor in the Black-Scholes model](mathematical-finance.md#guaranteed-terminal-stock-floor-in-the-black-scholes-model)
    - [Option vega](mathematical-finance.md#option-vega)
    - [Risk-neutral measure for the Black-Scholes model](mathematical-finance.md#risk-neutral-measure-for-the-black-scholes-model)
      - [Power payoff in the Black-Scholes model](mathematical-finance.md#power-payoff-in-the-black-scholes-model)
      - [Brownian time reversal for fixed-strike lookback extrema](mathematical-finance.md#brownian-time-reversal-for-fixed-strike-lookback-extrema)
    - [Black-Scholes formula](mathematical-finance.md#black-scholes-formula)
      - [Normalized Black-Scholes call function](mathematical-finance.md#normalized-black-scholes-call-function)
    - [Black-Scholes digital option formula](mathematical-finance.md#black-scholes-digital-option-formula)
      - [Digital put-call parity](mathematical-finance.md#digital-put-call-parity)
    - [Black-Scholes equation](mathematical-finance.md#black-scholes-equation)
      - [Separated solutions of the Black-Scholes equation](mathematical-finance.md#separated-solutions-of-the-black-scholes-equation)
      - [Black-Scholes equation with continuous stock dividends](mathematical-finance.md#black-scholes-equation-with-continuous-stock-dividends)
        - [Dividend-yield discount shift](mathematical-finance.md#dividend-yield-discount-shift)
      - [Black-Scholes equation with claim dividends](mathematical-finance.md#black-scholes-equation-with-claim-dividends)
      - [Black-Scholes value equation needs delta-compatible holdings](mathematical-finance.md#black-scholes-value-equation-needs-delta-compatible-holdings)
  - [Greeks (finance)](mathematical-finance.md#greeks-finance)
    - [Option theta](mathematical-finance.md#option-theta)
    - [Option delta](mathematical-finance.md#option-delta)
      - [Delta hedge](mathematical-finance.md#delta-hedge)
      - [Call delta equation for a driftless local volatility diffusion](mathematical-finance.md#call-delta-equation-for-a-driftless-local-volatility-diffusion)
        - [Derivative-weighted call delta martingale](mathematical-finance.md#derivative-weighted-call-delta-martingale)
  - [Implied volatility](mathematical-finance.md#implied-volatility)
    - [Black-Scholes implied volatility](mathematical-finance.md#black-scholes-implied-volatility)
  - [American option](mathematical-finance.md#american-option)
    - [American call option](mathematical-finance.md#american-call-option)
      - [Dividend-date call-exercise criterion](mathematical-finance.md#dividend-date-call-exercise-criterion)
      - [No early exercise of a call without dividends](mathematical-finance.md#no-early-exercise-of-a-call-without-dividends)
    - [American quadratic-payoff option in a binomial market](mathematical-finance.md#american-quadratic-payoff-option-in-a-binomial-market)
    - [Perpetual reciprocal-payoff American option](mathematical-finance.md#perpetual-reciprocal-payoff-american-option)
    - [American-option superhedge with a funded reserve](mathematical-finance.md#american-option-superhedge-with-a-funded-reserve)
  - [Modern portfolio theory](mathematical-finance.md#modern-portfolio-theory)
    - [Portfolio opportunity set](mathematical-finance.md#portfolio-opportunity-set)
    - [Gaussian two-fund theorem](mathematical-finance.md#gaussian-two-fund-theorem)
    - [Efficient frontier](mathematical-finance.md#efficient-frontier)
    - [Mean-variance efficient ray](mathematical-finance.md#mean-variance-efficient-ray)
      - [One-period Gaussian minimum-variance portfolio](mathematical-finance.md#one-period-gaussian-minimum-variance-portfolio)
    - [Gaussian one-fund theorem](mathematical-finance.md#gaussian-one-fund-theorem)
    - [Pareto dominance in mean-variance space](mathematical-finance.md#pareto-dominance-in-mean-variance-space)
    - [Mean-variance portfolio regression](mathematical-finance.md#mean-variance-portfolio-regression)
- [Positive-definite quadratic optimization](#positive-definite-quadratic-optimization)
  - [Orthogonal decomposition in a positive-definite metric](#orthogonal-decomposition-in-a-positive-definite-metric)

## Scheduling

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

Scheduling assigns jobs to processing resources and orders their execution subject to resource and precedence requirements. Objectives include completion time, lateness and throughput. In single-machine sequencing with all jobs mandatory, the total processing time is constant, but order-dependent setups can still change completion time. With parallel machines, machine allocation and sequencing jointly determine the [parallel-machine makespan with sequence-dependent setups](#parallel-machine-makespan-with-sequence-dependent-setups).

### Parallel-machine makespan with sequence-dependent setups

↑ **Parent:** [Scheduling](#scheduling)

Partition jobs between machines and choose an ordering on each machine. Machine $r$ has load $C_r$ equal to its processing times, initial setup and internal changeovers; the completion time of all jobs is the [maximum](set.md#maximum-of-a-subset-of-a-total-order) of these loads. Minimize a variable $C_{\max}$ subject to $C_r\leq C_{\max}$ for every machine. [Branch and bound](#branch-and-bound) can combine machine-assignment decisions with route bounds; heuristic moves relocate jobs between machines, swap jobs, and reorder blocks. Minimizing the sum of route costs alone does not generally minimize the makespan.

## Objective function

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

An [objective function](#objective-function) assigns a numerical score to each admissible decision. An optimization problem seeks a [feasible solution](#feasible-point) maximizing or minimizing this score.

// Target: mathematical-optimization.bigb

## Project scheduling

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

With unlimited parallel processing, a project is described by task durations and precedence constraints. A task can start only after its predecessors finish. For an acyclic precedence graph, minimizing total completion time amounts to finding a longest start-to-finish path.

// Target: mathematical-optimization.bigb

### Critical path method

↑ **Parent:** [Project scheduling](#project-scheduling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_path_method)

Add a dummy source before the initial tasks and a dummy sink after the terminal tasks. Give every arc leaving task $i$ length $\tau_i$, its duration, with zero duration at the source. The longest path length is the minimum possible project duration. Earliest starts are obtained in [topological order](combinatorics.md#topological-order) by $t_j=\max_{i\to j}(t_i+\tau_i)$. A longest path is a critical path.

// Target: mathematical-optimization.bigb

#### Project scheduling duality

↑ **Parent:** [Critical path method](#critical-path-method)

On the augmented precedence graph, the [linear programming](#linear-programming) problem

$$
\min(t_{\mathrm{sink}}-t_{\mathrm{source}})
\quad\text{subject to}\quad t_j-t_i\geq\tau_i
$$

has dual $\max\sum_{i\to j}\tau_i f_{ij}$, with $f\geq0$ a unit source-to-sink flow. Equivalently, the dual is the negative of the optimal [uncapacitated minimum-cost flow](graph-theory.md#uncapacitated-minimum-cost-flow) value with arc costs $-\tau_i$. The flow selects a longest path, while the time variables provide a matching [weak duality](#weak-duality) bound.

// Target: mathematical-optimization.bigb

##### Unit-flow certificate for project duration

↑ **Parent:** [Project scheduling duality](#project-scheduling-duality)

A feasible timetable with finish time $T$ and a unit flow carried on a precedence path of total duration $T$ certify optimality. Summing the inequalities $t_j-t_i\geq\tau_i$ along that path proves every schedule needs at least $T$, while the timetable attains it.

// Target: computer-science.bigb

## Maximum and minimum

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_and_minimum)

Maxima and minima are [extrema](#maximum-and-minimum) of a real-valued function. A global maximum of $f$ on its domain $D$ is a point $x_*$ with $f(x)\leq f(x_*)$ for every $x\in D$; a global minimum reverses the inequality. A local extremum requires the inequality only in a [neighbourhood](topology.md#neighbourhood-mathematics) of the point within $D$. In [constrained optimization](numerical-analysis.md#constrained-optimization), $D$ is the feasible set, so an extremum is tested relative to the constraints rather than in every ambient direction. Thus a constrained [local maximum](analysis.md#local-maximum) or [local minimum](analysis.md#local-minimum) can occur at a boundary point without being an interior [critical point](analysis.md#critical-point).

<h2 id="cobb-douglas-production-function">Cobb–Douglas production function</h2>

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cobb–Douglas_production_function)

For positive constants $A,\alpha,\beta$, a Cobb–Douglas production function describes output in terms of capital $K$ and labour $L$. It is homogeneous of degree $\alpha+\beta$. Under $K+wL=b$ with $b,w>0$, its unique nonnegative-input optimum is $K=\alpha b/(\alpha+\beta)$ and $L=\beta b/[w(\alpha+\beta)]$, obtained by maximizing the strictly concave logarithm along the budget line. The optimized output has derivative $(\alpha+\beta)\phi(b)/b$, equal to its budget [Lagrange multiplier](#lagrange-multiplier). When $\alpha+\beta>1$, the unconstrained Lagrangian supremum over the positive orthant is infinite for every finite multiplier, despite the finite constrained optimum; the global dual representation must not be presumed in this case.

## Heuristic optimization

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

[Heuristic optimization](#heuristic-optimization) seeks useful feasible solutions without necessarily providing a universal [approximation ratio](#approximation-ratio) or a polynomial worst-case guarantee. Examples are [local search](#local-search), [simulated annealing](#simulated-annealing) and [tabu search](#tabu-search). A claimed [approximation algorithm](#approximation-algorithm) needs a separate proved performance guarantee.

### Tabu search

↑ **Parent:** [Heuristic optimization](#heuristic-optimization)

[Tabu search](#tabu-search) keeps a short-term memory of recently reversed moves or visited attributes and prohibits them temporarily, reducing cycling in [local search](#local-search). It can select the best admissible neighbor even when that neighbor worsens the objective; an aspiration rule permits a tabu move when it improves the best known solution. For allocations, transfers and exchanges maintain feasibility and recent reverse transfers can be tabu.

### Simulated annealing

↑ **Parent:** [Heuristic optimization](#heuristic-optimization)

For a maximization objective, [simulated annealing](#simulated-annealing) accepts every improving proposed neighbor and accepts a worsening move of loss $\Delta$ with [probability](probability-theory.md#probability) $\exp(-\Delta/T)$ at temperature $T>0$. Decreasing the temperature reduces exploratory moves. Retain the best feasible solution seen. Finite practical cooling schedules carry no general global-optimality guarantee.

#### Likelihood-power annealing

↑ **Parent:** [Simulated annealing](#simulated-annealing)

To maximize a [log-likelihood](statistical-modelling.md#log-likelihood), use energy $-\ell$ and [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) proportional to $e^{\ell/T}=L^{1/T}$ at temperature $T>0$. Reversing this sign favors [likelihood](statistical-modelling.md#likelihood-function) minima and can make the [probability density function](continuous-probability-distribution.md#probability-density-function) nonnormalizable. For Poisson observations with total $s$ and sample size $m$, with respect to $d\lambda$ the normalized [probability density function](continuous-probability-distribution.md#probability-density-function) is

$$
\lambda\sim\operatorname{Gamma}(s/T+1,m/T).
$$

Its [mean](probability-theory.md#expected-value) is $(s+T)/m$ and [variance](variance.md) $(sT+T^2)/m^2$, so it concentrates at the [maximum-likelihood estimate](statistical-modelling.md#maximum-likelihood-estimator) $s/m$ as $T\downarrow0$. Cooling of equilibrium laws and convergence of a particular changing-temperature chain are different statements; the latter requires mixing or a direct chain argument.

##### Binomial likelihood-power annealing

↑ **Parent:** [Likelihood-power annealing](#likelihood-power-annealing)

For $m$ independent [binomial distribution](discrete-probability-distribution.md#binomial-distribution) observations with fixed trial count $n$ and total successes $s$, the likelihood-power [probability density function](continuous-probability-distribution.md#probability-density-function) relative to $dp$ is $p^{s/T}(1-p)^{(mn-s)/T}$. Its normalized law is the displayed [Beta distribution](probability-theory.md#beta-distribution). Its mean tends to $s/(mn)$ and its variance tends to zero as $T\downarrow0$, including endpoint maxima. Energy for maximizing a [log-likelihood](statistical-modelling.md#log-likelihood) is its negative; the opposite sign reverses the optimization.

##### Gaussian likelihood Gibbs annealing

↑ **Parent:** [Likelihood-power annealing](#likelihood-power-annealing)

Let $\bar x=m^{-1}\sum_i x_i$ and $S=\sum_i(x_i-\bar x)^2>0$. With Lebesgue base measure $d\mu\,dv$ for $v=\sigma^2$, the likelihood-power law has conditionals

$$
\mu\mid v\sim N(\bar x,Tv/m),\qquad
v\mid\mu\sim\operatorname{InvGamma}\left(\frac{m}{2T}-1,\frac{S+m(\mu-\bar x)^2}{2T}\right).
$$

The joint law is proper for $T<m/3$, since its marginal $v$ is [inverse-gamma distribution](continuous-probability-distribution.md#inverse-gamma-distribution) with shape $m/(2T)-3/2$ and scale $S/(2T)$. There is also a direct convergence proof for successive [Gibbs sampling](statistical-inference.md#gibbs-sampler) updates with deterministic $0<T_n\leq m/10$ and $T_n\to0$. Update $\mu_n$ from $v_{n-1}$, then $v_n$ from $\mu_n$. [Inverse-gamma distribution](continuous-probability-distribution.md#inverse-gamma-distribution) moments and conditional normal moments give

$$
\mathbb E v_n=\frac{S+T_n\mathbb E v_{n-1}}{m-4T_n},\qquad
\mathbb E v_n^2=\frac{S^2+2ST_n\mathbb E v_{n-1}+3T_n^2\mathbb E v_{n-1}^2}{(m-4T_n)(m-6T_n)}.
$$

The coefficients of the preceding moments are bounded by $1/6$ and $1/8$, so these moments stay bounded from a finite deterministic initial [variance](variance.md). Letting $T_n\to0$ gives $\mathbb E v_n\to S/m$ and $\mathbb E v_n^2\to(S/m)^2$. Also $\mathbb E(\mu_n-\bar x)^2=T_n\mathbb E v_{n-1}/m\to0$. Thus the iterates converge in [mean](probability-theory.md#expected-value) square to the normal [maximum-likelihood estimate](statistical-modelling.md#maximum-likelihood-estimator).

### Local search

↑ **Parent:** [Heuristic optimization](#heuristic-optimization)

[Local search](#local-search) repeatedly improves a feasible solution within a specified neighborhood until no improving move remains. For an allocation, neighbors can transfer an item or exchange items between bidders while preserving the partition. A local optimum need not be a global optimum; restarting from several initial solutions can explore different basins.

## Feasible point

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A feasible point satisfies every constraint of an optimization problem. For a [transportation problem](#transportation-problem) with capacity inequalities, feasibility requires nonnegative shipments, row totals no greater than factory capacities and column totals equal to shop demands. Feasibility alone does not prove minimal cost: a matching [transportation dual certificate with capacity inequalities](#transportation-dual-certificate-with-capacity-inequalities) provides an optimality proof. The set of all feasible points can be empty, and a finite infimum need not be attained even when the set is nonempty.

## Nonlinear programming

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonlinear_programming)

A [nonlinear programming](#nonlinear-programming) problem minimizes an objective over finitely many real variables subject to constraints, with at least one objective or constraint nonlinear. Parametrizing the pulse amplitudes in [quantum optimal control](control-theory.md#quantum-optimal-control) produces such a problem. [Gradient descent](numerical-analysis.md#gradient-descent) and related local methods exploit differentiability, but a local stationary point need not be a global optimum without additional convexity or other structure.

## Perturbation function

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A [perturbation function](#perturbation-function) encodes a family of objectives and constraints indexed by a perturbation $u$, with the original problem at $u=0$. Extended-real values encode constraints. Its marginal $p(u)=\inf_xf(x,u)$ measures the optimal value's response to perturbation; jointly convex data give [convex perturbation duality](#convex-perturbation-duality).

## Chance constraint

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A constraint imposed with a specified [probability](probability-theory.md#probability) when data or demands are random. Distributional assumptions can turn it into a deterministic condition on decision variables. The choice of strict versus non-strict event matters when the distribution has atoms, as in the [deterministic boundary in an upper-tail chance constraint](#deterministic-boundary-in-an-upper-tail-chance-constraint).

### Deterministic boundary in an upper-tail chance constraint

↑ **Parent:** [Chance constraint](#chance-constraint)

A deterministic demand has [probability](probability-theory.md#probability) one of meeting or exceeding its mean. Thus replacing a positive-variance [Gaussian chance constraint](#exact-gaussian-chance-constraint) by its naive zero-variance limit with a non-strict capacity inequality loses the boundary condition. The example $X=0$, $C=0$, $\varepsilon=e^{-1}$ satisfies $m+\phi\sqrt v\leq C$ for finite $\phi$, but violates the chance requirement.

### Exact Gaussian chance constraint

↑ **Parent:** [Chance constraint](#chance-constraint)

For $X\sim N(m,v)$ with $v>0$ and $0<\varepsilon<1$, $P(X\geq C)\leq\varepsilon$ is equivalent to the displayed [chance constraint](#chance-constraint), because the [standard normal distribution function](probability-theory.md#standard-normal-distribution-function) is continuous and strictly increasing. The coefficient is a [standard normal quantile](probability-theory.md#standard-normal-quantile), which can be negative. If $v=0$, equality is an atom and the exact condition becomes $C>m$ instead.

## Variational inequality

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

For a feasible set $K$ and a vector field $F$, a [variational inequality](#variational-inequality) asks for $x^*\in K$ satisfying the displayed inequality for every feasible $x$. If $K$ is convex and $F$ is the gradient of a differentiable [convex function](real-analysis.md#convex-function), it is the necessary and sufficient first-order condition for minimizing that function. It also describes [Wardrop equilibria](queueing-theory.md#wardrop-equilibrium) when no scalar objective has the route-cost vector as its gradient.

## First-order optimality condition

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

At an interior local extremum of a [differentiable function](analysis.md#differentiable-function), its [gradient](calculus.md#gradient) is zero: restricting the function to every line through the point shows that all directional derivatives vanish. This is only a necessary condition in general. For a [strictly concave function](real-analysis.md#strictly-concave-function), an interior stationary point is the unique global maximizer on its convex domain. Constrained or boundary optima instead need conditions adapted to their feasible directions.

## Lagrangian duality

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

For a [minimization problem](#minimization-problem), the infimum of the [optimization Lagrangian](#optimization-lagrangian) over its primal variables gives a lower bound for each allowable multiplier. Maximizing these lower bounds is the [Lagrangian dual problem](#lagrangian-dual-problem). [Weak duality](#weak-duality) always holds; [strong duality](#strong-duality) requires further hypotheses and holds for feasible bounded [linear programs](#linear-programming).

### Strong Lagrangian property

↑ **Parent:** [Lagrangian duality](#lagrangian-duality)

For a finite constrained optimum value $\phi(b)=\inf\{f(x):h(x)=b,x\in X\}$ and [optimization Lagrangian](#optimization-lagrangian) $L_b(x,\lambda)=f(x)-\lambda^T(h(x)-b)$, the strong Lagrangian property means that some finite [Lagrange multiplier](#lagrange-multiplier) attains the dual lower bound exactly: $\inf_XL_b=\phi(b)$. It includes dual attainment, but need not include primal attainment. It is equivalent to a [non-vertical supporting hyperplane of a value function](#non-vertical-supporting-hyperplane-of-a-value-function): a supporting slope gives $f(x)\geq\phi(h(x))\geq\phi(b)+\lambda^T(h(x)-b)$, hence $\inf_XL_b\geq\phi(b)$; [weak duality](#weak-duality) gives the opposite inequality. Conversely the infimum identity bounds every $L_b(x,\lambda)$ below by $\phi(b)$; taking the infimum over $h(x)=u$ gives the supporting inequality. No convexity assumption is needed for this equivalence.

### Primal problem

↑ **Parent:** [Lagrangian duality](#lagrangian-duality)

The original [mathematical optimization](mathematical-optimization.md) problem relative to a chosen [Lagrangian dual problem](#lagrangian-dual-problem). In [convex perturbation duality](#convex-perturbation-duality), its objective is $\varphi(x)=f(x,0)$ and its value is $p(0)$. [Strong duality](#strong-duality) concerns optimal values; primal attainment additionally requires an actual minimizing point.

## Maximization problem

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A maximization problem seeks a feasible point with largest objective value. Its supremum can fail to be attained or be infinite. Negating the objective gives a [minimization problem](#minimization-problem). A global extremum of an [optimization Lagrangian](#optimization-lagrangian) can certify a feasible optimum by the [Lagrangian sufficiency theorem](#lagrange-sufficiency-theorem).

## Minimization problem

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A minimization problem seeks a feasible point with smallest objective value. Its infimum can be finite without being attained, or equal to $-\infty$ when unbounded below. Negating the objective converts it to a [maximization problem](#maximization-problem).

## Parametric optimization

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A parametric optimization problem has objective or constraints depending on input data. Its optimizer set is a [solution map of a parametric optimization problem](#solution-map-of-a-parametric-optimization-problem). [Sensitivity analysis](probability-and-statistics.md#sensitivity-analysis) asks how this map changes as the data vary.

### Solution map of a parametric optimization problem

↑ **Parent:** [Parametric optimization](#parametric-optimization)

The solution map sends a data parameter $a$ to the set of minimizers of the associated objective, $S(a)=\operatorname{argmin}_x F_a(x)$. Existence, uniqueness and local stability are distinct questions. Strong convexity gives uniqueness when a minimizer exists; the [Aubin property](#aubin-property) gives a perturbation bound.

## Variational analysis

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variational_analysis)

Variational analysis studies optimization, perturbation stability and generalized differentiation through functions, sets and [set-valued mappings](#set-valued-mapping). [Convex analysis](convex-optimization.md#convex-analysis) is a foundational special case; limiting normal constructions also handle nonconvex geometry.

### Normal cone

↑ **Parent:** [Variational analysis](#variational-analysis)

Normal cones describe generalized supporting directions to sets. For a convex set, the normal condition is $\langle w,z^\prime-z\rangle\leq0$ for every $z^\prime$ in the set. For nonconvex sets, the [Fréchet normal cone](#frechet-normal-cone) and the [limiting normal cone](#limiting-normal-cone) distinguish local regular support from limits of such supports.

#### Limiting normal cone

↑ **Parent:** [Normal cone](#normal-cone)

The limiting normal cone consists of limits $w_k\to w$ of vectors from the [Fréchet normal cone](#frechet-normal-cone) $w_k\in\widehat N_C(z_k)$ with $z_k\to z$ in $C$. It need not be convex. Including normals from nearby graph pieces is essential to the [Mordukhovich criterion](#mordukhovich-criterion).

<h4 id="frechet-normal-cone">Fréchet normal cone</h4>

↑ **Parent:** [Normal cone](#normal-cone)

A vector $w$ is a regular normal at $z\in C$ when $\limsup_{z^\prime\to z,\ z^\prime\in C\setminus\{z\}}\langle w,z^\prime-z\rangle/\|z^\prime-z\|\leq0$. At an isolated point all vectors satisfy this condition. It is the local first-order supporting cone.

### Set-valued analysis

↑ **Parent:** [Variational analysis](#variational-analysis)

Set-valued analysis studies relations whose output at one input is a set. Solution maps, [subdifferentials](convex-optimization.md#subdifferential) and generalized normal mappings are important examples. Graph geometry provides definitions of continuity, local stability and differentiation.

#### Set-valued mapping

↑ **Parent:** [Set-valued analysis](#set-valued-analysis)

A mapping $S:X\rightrightarrows Y$ assigns a subset $S(u)\subset Y$ to each $u$. Empty and multiple values are allowed. The [graph of a set-valued mapping](#graph-of-a-set-valued-mapping) records the relation as a subset of $X\times Y$.

##### Upper hemicontinuity

↑ **Parent:** [Set-valued mapping](#set-valued-mapping)

A [set-valued mapping](#set-valued-mapping) $F$ is upper hemicontinuous at $x$ when every open set containing $F(x)$ also contains $F(x')$ for all nearby $x'$. With values in a fixed [compact](topology.md#compact-space) space, a closed [graph of a set-valued mapping](#graph-of-a-set-valued-mapping) implies [upper hemicontinuity](#upper-hemicontinuity): a violating sequence has a convergent subsequence of outputs whose limit lies in the limiting value.

##### Aubin property

↑ **Parent:** [Set-valued mapping](#set-valued-mapping)

Near $(\bar u,\bar v)$ in a graph, this property requires neighborhoods $U,V$ and a finite $\kappa$ such that $S(u)\cap V\subset S(u^\prime)+\kappa\|u-u^\prime\|\mathbb B$ for all $u,u^\prime\in U$. Nearby solutions can be matched under nearby perturbations with linear displacement control. Single-valued maps reduce to local [Lipschitz continuity](real-analysis.md#lipschitz-continuity).

###### Mordukhovich criterion

↑ **Parent:** [Aubin property](#aubin-property)

In finite dimensions, if the graph is locally closed at $(\bar u,\bar v)$, the [Aubin property](#aubin-property) holds exactly when $D^*S(\bar u\mid\bar v)(0)=\{0\}$. Thus no nonzero horizontal vector in the [limiting normal cone](#limiting-normal-cone) may occur. The exact local Lipschitz modulus is the outer norm of this [coderivative](#limiting-coderivative).

##### Graph of a set-valued mapping

↑ **Parent:** [Set-valued mapping](#set-valued-mapping)

The graph is $\operatorname{gph}S=\{(u,v):v\in S(u)\}$. Local graph normals encode the [Mordukhovich coderivative](#limiting-coderivative) and hence the [Aubin property](#aubin-property). Graph closedness is a local hypothesis in the sensitivity criterion.

###### Limiting coderivative

↑ **Parent:** [Graph of a set-valued mapping](#graph-of-a-set-valued-mapping)

The limiting coderivative is $D^*S(\bar u\mid\bar v)(v^*)=\{u^*:(u^*,-v^*)\in N_{\operatorname{gph}S}(\bar u,\bar v)\}$. The negative sign on the output dual is essential. For a smooth single-valued function it gives the transpose Jacobian acting on $v^*$.

## Pareto efficiency

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

An outcome is Pareto efficient when no feasible alternative weakly improves every agent's utility and strictly improves at least one. For strict preference orders over distinct alternatives, an outcome unanimously ranked below another is inefficient. Onto [strategyproof](game-theory.md#strategyproofness) [social choice functions](game-theory.md#social-choice-function) on an unrestricted domain are Pareto efficient: rank-raising monotonicity and unanimity rule out selecting a unanimously dominated alternative.

### Pairwise improvement from nonparallel utility gradients

↑ **Parent:** [Pareto efficiency](#pareto-efficiency)

Two strictly positive nonproportional utility gradients $g,h$ admit a transfer direction $\delta$ with $g\cdot\delta>0$ and $h\cdot\delta<0$. Choose $\delta=g-th$ with $(g\cdot h)/\|h\|^2<t<\|g\|^2/(g\cdot h)$; strict [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) makes this interval nonempty. Small opposite transfers in this direction strictly improve both differentiable utilities. Absence of such trades therefore forces positive proportionality of all gradients in an unconstrained allocation space.

### Pareto frontier

↑ **Parent:** [Pareto efficiency](#pareto-efficiency)

The Pareto frontier consists of feasible payoff vectors that no other feasible vector weakly improves in every coordinate and strictly improves in at least one. A [Nash bargaining solution](game-theory.md#nash-bargaining-solution) with positive gains lies on this frontier, because increasing either gain without decreasing the other raises its [Nash product](game-theory.md#nash-product).

## Approximation algorithm

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

An approximation algorithm efficiently returns a feasible solution with a proved performance guarantee relative to the optimum. The guarantee must specify whether the problem is a maximization or minimization problem.

### Fully polynomial randomized approximation scheme

↑ **Parent:** [Approximation algorithm](#approximation-algorithm)

For a nonnegative counting quantity $Z$, an FPRAS is a [randomized algorithm](computer-science.md#randomized-algorithm) with the displayed guarantee, running in time polynomial in encoded input length, $\varepsilon^{-1}$ and $\log(\delta^{-1})$. The usual constant-success definition is equivalent by independent repetition and a median. This counting notion differs from a deterministic [fully polynomial-time approximation scheme](#fully-polynomial-time-approximation-scheme) for optimization.

### Fully polynomial-time approximation scheme

↑ **Parent:** [Approximation algorithm](#approximation-algorithm)

For every $\varepsilon>0$, such a scheme returns a feasible solution within relative error $\varepsilon$ and runs in time polynomial in the encoded instance size and in $1/\varepsilon$. Dependence polynomial only for each fixed epsilon is the weaker polynomial-time approximation-scheme requirement.

### Approximation ratio

↑ **Parent:** [Approximation algorithm](#approximation-algorithm)

For maximization, an approximation ratio $\alpha\in(0,1]$ means the returned feasible value is at least $\alpha$ times the optimal value on every permitted instance. Some conventions instead report its reciprocal; specify the convention.

#### Relative-error approximation for minimization

↑ **Parent:** [Approximation ratio](#approximation-ratio)

For a minimization problem with positive optimum, this convention measures the relative excess $(\operatorname{ALG}-\operatorname{OPT})/\operatorname{OPT}$. An epsilon-approximation always returns a feasible solution with excess at most $\varepsilon$. A multiplicative-ratio convention instead reports $1+\varepsilon$. State the convention explicitly rather than treating these two numbers as interchangeable.

## Integer programming

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

An integer program optimizes an objective under constraints with some or all variables restricted to integers. Its continuous relaxation removes those integrality restrictions; a relaxed optimum bounds the integer optimum in the appropriate direction.

### Two-bin load balancing

↑ **Parent:** [Integer programming](#integer-programming)

Partition positive item weights into two bins to minimize the heavier total. The optimum is at least both half the total weight and the largest individual weight. This is two-machine makespan minimization, rather than the version of bin packing that minimizes the number of fixed-capacity bins.

#### Rounded dynamic programming for two-bin load balancing

↑ **Parent:** [Two-bin load balancing](#two-bin-load-balancing)

For integer weights, subset-sum [dynamic programming](#dynamic-programming) finds the greatest achievable total at most $s/2$ in time $O(ns)$, where $s$ is the total weight. For rational weights and $0<\varepsilon<1$, scale by $K=\varepsilon s/(2n)$ and round down to $q_i=\lfloor w_i/K\rfloor$. The scaled total is at most $2n/\varepsilon$, so exact dynamic programming costs $O(n^2/\varepsilon)$ arithmetic operations. Lifting its partition to the original weights increases the maximum load by at most $nK\leq\varepsilon\operatorname{OPT}$. Thus it is a [fully polynomial-time approximation scheme](#fully-polynomial-time-approximation-scheme) for this two-bin problem. Bit complexity also accounts for the rational input and epsilon encodings.

#### Greedy two-bin scheduling bound

↑ **Parent:** [Two-bin load balancing](#two-bin-load-balancing)

Put each successive item into a currently lighter bin. Before receiving weight $w_j$, that bin contains at most half the total weight already assigned, hence at most $(s-w_j)/2$, where $s$ is the overall total. Apply this to the last item in a finally heaviest bin to get $\operatorname{ALG}\leq s/2+w_{\max}/2$. Since $\operatorname{OPT}\geq\max(s/2,w_{\max})$, the approximation ratio is at most $3/2$. Ordered weights $1,1,2$ give loads $3,1$ rather than the optimal $2,2$, proving the bound is sharp. Its relative-error guarantee is $\varepsilon=1/2$.

### Small integer feasibility witness by homogeneous cone decomposition

↑ **Parent:** [Integer programming](#integer-programming)

If $Bz=b$, $z\geq0$ has an integer solution, with $N$ variables and all data bounded by $M\geq1$, it has one satisfying the displayed bound. Apply [support-minimal rays of a nonnegative kernel](#support-minimal-rays-of-a-nonnegative-kernel) to $(z,1)$ in the cone $\{(u,t)\geq0:Bu=bt\}$. Its integer generators have coordinates bounded by $D=(N+1)!M^{N+1}$. Generators with positive last coordinate normalize to feasible points with coordinates at most $D$; their coefficients form a convex combination. The remaining generators are integer recession directions. Subtract the integer parts of their coefficients from the original integer solution. The result remains integral and feasible and has coordinates at most $D+(N+1)D$. Its binary length is polynomial in the input size. Splitting unrestricted integer variables and adding integer slacks reduces general integer linear feasibility to this form, proving its membership in [NP](computer-science.md#np-complexity).

### Winner determination problem

↑ **Parent:** [Integer programming](#integer-programming)

Given bidders' values $v_i(S)$ for item bundles, the [winner determination problem](#winner-determination-problem) maximizes $\sum_i v_i(S_i)$ over disjoint allocated bundles. When every item must be assigned, the bundles form a partition. General values permit complements and difficult combinatorial search; monotone [submodular set functions](function.md#submodular-set-function) permit a greedy half-approximation. Complexity claims must specify whether the values are supplied explicitly or by a value oracle.

#### Greedy half-approximation for submodular welfare

↑ **Parent:** [Winner determination problem](#winner-determination-problem)

Allocate each remaining item to a bidder with greatest current marginal gain. For nonnegative monotone [submodular set functions](function.md#submodular-set-function), this uses $O(mn^2)$ value queries and achieves the displayed guarantee. To prove it by induction, let the first allocation give item $j$ to bidder $r$, and set $w=v_r(\{j\})$. Contract that item into bidder $r$'s value by replacing it with $v'_r(S)=v_r(S\cup\{j\})-w$ and leave the other bidders' values unchanged. The remaining greedy run is identical, and $A(v)=w+A(v')$. Move $j$ from its owner in an optimal allocation to $r$. [Submodularity](function.md#submodular-set-function) bounds the owner's loss by its initial singleton marginal, which is no larger than the selected greedy marginal and hence no larger than $w$. The receiver's value cannot decrease, so $\operatorname{Opt}(v')\geq\operatorname{Opt}(v)-2w$. Induction proves the guarantee, with the zero-item case immediate even for nonzero empty-bundle values.

### Quadratic assignment problem

↑ **Parent:** [Integer programming](#integer-programming)

A [permutation](combinatorics.md#permutation) assigns facilities to locations, and the objective combines their pairwise interactions with pairwise location costs. Ordered-pair and unordered-pair conventions differ by a factor of two for symmetric data. The decision version is [NP-complete](computer-science.md#np-completeness): letting $A$ record a directed cycle makes the objective exactly the length of a [travelling salesman problem](#travelling-salesman-problem) tour under the ordering given by the [permutation](combinatorics.md#permutation). The optimization version is [NP-hard](computer-science.md#np-hardness).

#### Gilmore-Lawler bound

↑ **Parent:** [Quadratic assignment problem](#quadratic-assignment-problem)

For each facility $i$ and location $k$, independently minimize its row contribution over bijections from the other facilities to the other locations, giving $\ell_{ik}$. Every complete assignment has row contribution at least its corresponding $\ell_{ik}$, so minimizing their sum is a lower bound on the quadratic objective. Fixed assignments are retained as constraints in this [assignment problem](#assignment-problem), which the [Hungarian algorithm](#hungarian-algorithm) solves. The independently optimal rows need not be simultaneously realizable, explaining why the bound can be strict.

### Branch and bound

↑ **Parent:** [Integer programming](#integer-programming)

A branch-and-bound search partitions a feasible set, maintains a feasible incumbent, and prunes subproblems using bounds that cannot improve that incumbent. For a [quadratic knapsack problem](#quadratic-knapsack-problem), fixing a selected set $S$ adds its exact quadratic value as a constant and replaces remaining profits by $v_i+2\sum_{j\in S}p_{ij}$ under the ordered-pair convention. Residual [fractional row bounds for quadratic knapsack](#fractional-row-bound-for-quadratic-knapsack) and a [Lagrangian knapsack bound](#lagrangian-knapsack-bound) can then be recomputed. Worst-case search remains exponential.

#### Incumbent solution

↑ **Parent:** [Branch and bound](#branch-and-bound)

An [incumbent solution](#incumbent-solution) is the best feasible solution found so far by an optimization search. Its objective value is an upper bound on a minimization optimum and a lower bound on a maximization optimum; bounds on unexplored subproblems can be compared with it to prune the search.

// Target: combinatorics.bigb

#### Best-bound search

↑ **Parent:** [Branch and bound](#branch-and-bound)

For minimization, [best-bound search](#best-bound-search) expands the active [branch and bound](#branch-and-bound) node with smallest [lower bound](set.md#lower-bound-in-a-partially-ordered-set). A feasible completed assignment supplies an incumbent upper bound. Nodes with lower bound at least that incumbent can be discarded when only one optimum is needed. Search ends with an optimality certificate when no active node can improve the incumbent.

// Target: combinatorics.bigb

### Knapsack problem

↑ **Parent:** [Integer programming](#integer-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knapsack_problem)

The knapsack problem selects items of prescribed weights and profits under a total-weight capacity. The [0-1 knapsack problem](#0-1-knapsack-problem) permits each item at most once; bounded and unbounded multiplicity variants use different integer restrictions. Nonnegative weights and capacity are assumed here.

#### Quadratic knapsack problem

↑ **Parent:** [Knapsack problem](#knapsack-problem)

The quadratic knapsack problem includes pairwise interactions between selected items. For symmetric $p_{ij}$, a sum over all ordered pairs counts each unordered interaction twice; an alternative convention sums only over $i<j$. The objective convention must be kept consistent when bounding or fixing variables.

##### Fractional row bound for quadratic knapsack

↑ **Parent:** [Quadratic knapsack problem](#quadratic-knapsack-problem)

Conditioning on selecting item $i$ leaves capacity $B-w_i$. Its [fractional knapsack problem](#fractional-knapsack-problem) bounds that item's total interaction with the other selected items. Thus the ordered-pair quadratic objective is at most $\sum_i(v_i+q_i)x_i$. Remove overweight items before defining their residual-capacity problems.

#### Fractional knapsack problem

↑ **Parent:** [Knapsack problem](#knapsack-problem)

This [linear programming](#linear-programming) relaxation allows a fraction of each item. With positive weights, sort decreasing profit-to-weight ratios and fill capacity in that order, using at most one fractional item. An exchange argument proves optimality. Negative-profit items are omitted and positive-profit zero-weight items are included for free.

#### 0-1 knapsack problem

↑ **Parent:** [Knapsack problem](#knapsack-problem)

This binary [integer program](#integer-programming) selects each item at most once. Exact optimization is [NP-hard](computer-science.md#np-hardness); the [fractional knapsack problem](#fractional-knapsack-problem) gives an upper bound and supports a [half-approximation algorithm for knapsack](#half-approximation-algorithm-for-knapsack).

##### Half-approximation algorithm for knapsack

↑ **Parent:** [0-1 knapsack problem](#0-1-knapsack-problem)

After removing overweight items and handling free items, compare the feasible density-sorted prefix with the best feasible singleton. The [fractional knapsack problem](#fractional-knapsack-problem) optimum is at most the sum of their profits, so the better solution has [approximation ratio](#approximation-ratio) $1/2$.

### Cutting-plane method

↑ **Parent:** [Integer programming](#integer-programming)

A cutting-plane method repeatedly adds valid inequalities that exclude a current relaxed solution while preserving all feasible integer solutions. [Gomory fractional cuts](#gomory-fractional-cut) provide such inequalities from a fractional [simplex dictionary](numerical-analysis.md#simplex-dictionary).

#### Gomory fractional cut

↑ **Parent:** [Cutting-plane method](#cutting-plane-method)

For an all-integer dictionary row $x_B+\sum_j a_jx_j=b$ with nonnegative variables, this cut follows because $x_B+\sum_j\lfloor a_j\rfloor x_j$ is an integer and $\sum_j\{a_j\}x_j\geq0$. Consequently that integer is at most $\lfloor b\rfloor$. Negative coefficients use the usual [fractional part](calculus.md#fractional-part) $u-\lfloor u\rfloor$, so $\{-1/5\}=4/5$. Normalize a resulting inequality sensibly before introducing a new integer-valued [slack variable](#slack-variable).

##### Gomory infeasibility certificate from a fractional slack row

↑ **Parent:** [Gomory fractional cut](#gomory-fractional-cut)

For a nonnegative all-integer row $x_B+\sum_j a_jx_j=b$ with $a_j>0$, the [Gomory fractional cut](#gomory-fractional-cut) requires $\sum_j\{a_j\}x_j\geq\{b\}$. The original row gives $\sum_j a_jx_j\leq b$. If a constant $\kappa$ satisfies $\{a_j\}\leq\kappa a_j$ for every $j$ and $\kappa b<\{b\}$, these inequalities contradict the cut. A single row therefore certifies integer infeasibility. Slacks may be used as integer variables when the original constraint coefficients and right sides are integral and the decision variables are integral.

## Travelling salesman problem

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Travelling_salesman_problem)

Given finitely many locations and pairwise travel costs, find a cyclic visiting order minimizing the sum of its costs. For [Euclidean distance](topological-analysis.md#euclidean-distance) this becomes the [Euclidean travelling salesman tour](#euclidean-travelling-salesman-tour) problem.

### Assignment relaxation of the travelling salesman problem

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

Minimizing $\sum_{ij}c_{ij}x_{ij}$ over binary variables with one outgoing and one incoming edge at every [graph vertex](graph.md#vertex-graph-theory), and $x_{ii}=0$, is an [assignment problem](#assignment-problem). Its feasible solutions are [cycle covers of a directed graph](graph-theory.md#cycle-cover-of-a-directed-graph), whereas a [travelling salesman problem](#travelling-salesman-problem) requires one [Hamiltonian cycle](graph-theory.md#hamilton-cycle). The relaxed minimum is therefore a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) on the tour cost. If its optimum contains a proper subtour $C$, every tour omits at least one edge of $C$. Branching into subproblems that respectively forbid each edge of $C$ preserves every possible tour. Solving each child [assignment problem](#assignment-problem) and pruning those whose bounds exceed the best tour yields a finite [branch and bound](#branch-and-bound) algorithm. Equality also permits pruning when only one optimum is wanted.

### 2-opt

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/2-opt)

A 2-opt tour move removes two boundary arcs and reverses the intervening block to reconnect one tour. Such moves define a local-search neighbourhood; block reversals of length two include adjacent swaps and hence connect permutation schedules. For directed costs the [asymmetric 2-opt reversal cost](#asymmetric-2-opt-reversal-cost) must include every reversed internal arc, not just the boundary changes.

#### Asymmetric 2-opt reversal cost

↑ **Parent:** [2-opt](#2-opt)

A 2-opt schedule move reverses a consecutive block $v_p,\ldots,v_q$, reconnecting its boundary arcs. With directed costs, its change is

$$
\Delta=c_{v_{p-1},v_q}+c_{v_p,v_{q+1}}
-c_{v_{p-1},v_p}-c_{v_q,v_{q+1}}
+\sum_{r=p}^{q-1}(c_{v_{r+1},v_r}-c_{v_r,v_{r+1}}).
$$

Omitting the internal sum is valid only for symmetric costs. A [simulated annealing](#simulated-annealing) step accepts an increase with probability $\exp(-\Delta/T)$; a strictly positive temperature permits escape from local minima.

### Dummy-job reduction for sequence-dependent setup times

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

Add a dummy job $0$. Give the arc $0\to i$ cost equal to job $i$'s initial setup, the arc $i\to j$ its changeover cost, and every arc $i\to0$ zero cost. A [Hamiltonian cycle](graph-theory.md#hamilton-cycle) through the dummy represents a schedule, starting just after $0$ and ending just before it. The total processing time is constant on a single machine, so minimizing cycle cost minimizes completion time. Dropping [subtour elimination constraints](#subtour-elimination-constraints) gives an [assignment problem](#assignment-problem) lower bound.

### Subtour elimination constraints

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

Binary arc variables with one outgoing and one incoming arc at each vertex describe a [cycle cover of a directed graph](graph-theory.md#cycle-cover-of-a-directed-graph). For every nonempty proper vertex subset $S$, the displayed inequality forbids a directed cycle confined to $S$. Together these inequalities make the cycle cover one [Hamiltonian cycle](graph-theory.md#hamilton-cycle). They can be generated as violated cuts or used in [branch and bound](#branch-and-bound), rather than all being stored initially.

### Compact order formulation of the travelling salesman problem

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

Use binary directed-edge variables $x_{ij}$, one incoming and one outgoing edge at each city, and integer order variables $1\leq u_i\leq n-1$ for cities other than a distinguished city. The constraints $u_i-u_j+(n-1)x_{ij}\leq n-2$ for distinct nondistinguished cities force order increase along every selected edge away from the distinguished city. Summing around any cycle avoiding that city gives a contradiction, so the degree equations describe a single tour. There are $O(n^2)$ nonzero constraint entries apart from the degree equations, also totaling $O(n^2)$ entries. With costs at most $2^n$, the objective requires $O(n^3)$ bits and the remaining sparse constraint encoding $O(n^2\log n)$ bits. Omitting zero matrix entries is essential for this particular size bound.

### Max-TSP

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

Find a maximum-weight [Hamiltonian cycle](graph-theory.md#hamilton-cycle) in a complete weighted [graph](graph.md) or complete [directed graph](graph-theory.md#directed-graph). Nonnegative weights admit a [cycle-cover patching half-approximation for Max-TSP](#cycle-cover-patching-half-approximation-for-max-tsp) without a [triangle inequality](topological-analysis.md#triangle-inequality). For integer weights, changing $c_{ij}$ to $M-c_{ij}$, with $M\geq\max c_{ij}$, changes an $n$-vertex tour's weight from $C$ to $nM-C$. Consequently the strict-threshold decision version is [NP-complete](computer-science.md#np-completeness): minimum-tour threshold $C\leq L$ becomes maximum-tour threshold $C'>nM-L-1$.

#### Cycle-cover patching half-approximation for Max-TSP

↑ **Parent:** [Max-TSP](#max-tsp)

Solve the maximum-weight [assignment problem](#assignment-problem) forbidding fixed points, obtaining a [cycle cover of a directed graph](graph-theory.md#cycle-cover-of-a-directed-graph) whose weight bounds every [Hamiltonian cycle](graph-theory.md#hamilton-cycle) above. Remove a lightest [edge](graph-theory.md#edge-of-a-graph) from each [graph cycle](graph-theory.md#cycle-in-a-graph). Each [graph cycle](graph-theory.md#cycle-in-a-graph) has at least two [edges](graph-theory.md#edge-of-a-graph), so at least half its nonnegative weight survives. Connect the resulting disjoint [graph paths](graph-theory.md#path-in-a-graph) cyclically; completeness supplies the connectors and their nonnegative weights cannot reduce the retained sum. The [Hungarian algorithm](#hungarian-algorithm) and linear-time patching give a [polynomial time](computer-science.md#polynomial-time) [approximation algorithm](#approximation-algorithm). Negative weights invalidate a universal multiplicative half guarantee: when every weight is $-1$, every tour has weight $-n<(-n)/2$.

### Metric travelling salesman problem

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

This is the [travelling salesman problem](#travelling-salesman-problem) on a complete graph with nonnegative symmetric distances satisfying the [triangle inequality](topological-analysis.md#triangle-inequality). Repeated visits can be shortcut without increasing cost. Assigning distance one to edges of an input graph and two to its nonedges creates a metric instance with a tour of cost at most the number of vertices exactly when the graph has a [Hamiltonian cycle](graph-theory.md#hamilton-cycle). Thus the metric problem remains [NP-hard](computer-science.md#np-hardness).

#### Double-tree approximation for metric TSP

↑ **Parent:** [Metric travelling salesman problem](#metric-travelling-salesman-problem)

Double every edge of a [minimum spanning tree](combinatorics.md#minimum-spanning-tree) to obtain a connected even-degree multigraph, traverse an [Euler circuit](graph-theory.md#euler-circuit), and shortcut repeated vertices. The [triangle inequality](topological-analysis.md#triangle-inequality) prevents any shortcut from increasing cost. Deleting an edge of an optimal tour gives a spanning tree, so the minimum spanning tree has cost at most the optimal tour. The returned tour therefore costs at most twice optimum and is computable in polynomial time. In the relative-error convention this is an error-one approximation.

#### Christofides algorithm

↑ **Parent:** [Metric travelling salesman problem](#metric-travelling-salesman-problem)

Compute a [minimum spanning tree](combinatorics.md#minimum-spanning-tree), then a [minimum-weight perfect matching](graph-theory.md#minimum-weight-perfect-matching) on its odd-degree vertices. Their multiset union is connected with even degrees, so it has an [Euler circuit](graph-theory.md#euler-circuit). Shortcut repeated vertices to obtain a metric tour. The tree costs at most the optimal tour, and shortcutting the optimal tour to its odd-degree subset gives a cyclic order whose alternating matchings show that the added matching costs at most half the optimum. The result is a polynomial-time $3/2$-[approximation algorithm](#approximation-algorithm) for symmetric metric instances.

### Euclidean travelling salesman tour

↑ **Parent:** [Travelling salesman problem](#travelling-salesman-problem)

A closed polygonal tour through a finite point set, measured using [Euclidean distance](topological-analysis.md#euclidean-distance). Write $\operatorname{TS}(X)$ for the minimum length over cyclic visiting orders. A two-point tour traverses its segment twice; a one-point tour has length zero. The [triangle inequality](topological-analysis.md#triangle-inequality) allows repeated visits to be shortcut when estimating this minimum.

#### Weighted mismatch bound for Euclidean tours

↑ **Parent:** [Euclidean travelling salesman tour](#euclidean-travelling-salesman-tour)

For every configuration $x$ in the unit square there are nonnegative weights $a_i(x)$ such that $\sum_i a_i(x)^2\leq16$ and

$$
\operatorname{TS}(x)-\operatorname{TS}(y)\leq\sum_{i:x_i\ne y_i}a_i(x)\quad\text{for every }y.
$$

Use the sums of the two incident edge lengths in a tour from the [squared edge bound for tours in the unit square](#squared-edge-bound-for-tours-in-the-unit-square). Runs of missing vertices can be added by the cheaper of two out-and-back detours. This connects [Euclidean travelling salesman tours](#euclidean-travelling-salesman-tour) to [Talagrand's convex distance inequality](probability-inequality.md#talagrand-s-convex-distance-inequality).

#### Squared edge bound for tours in the unit square

↑ **Parent:** [Euclidean travelling salesman tour](#euclidean-travelling-salesman-tour)

Every finite point set in the unit square admits a cyclic visiting order with $\sum_i\lVert x_{i+1}-x_i\rVert^2\leq4$. Split the square into two [right triangles](geometry-and-topology.md#right-triangle), apply the [quadratic path bound in a right triangle](#quadratic-path-bound-in-a-right-triangle), and remove auxiliary corners using the [law of cosines](geometry-and-topology.md#law-of-cosines). The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) then gives $\operatorname{TS}(X)\leq2\sqrt{|X|}$. The tour minimizing ordinary length need not minimize the sum of squared lengths.

##### Quadratic path bound in a right triangle

↑ **Parent:** [Squared edge bound for tours in the unit square](#squared-edge-bound-for-tours-in-the-unit-square)

Given finitely many points in a [right triangle](geometry-and-topology.md#right-triangle) with hypotenuse endpoints $a,b$, there is a path from $a$ to $b$ visiting them all with sum of squared edge lengths at most $\lVert a-b\rVert^2$. Repeated altitude subdivision reduces to cells containing one point. Joining the child paths preserves the squared-cost bound by the [Pythagorean theorem](geometry-and-topology.md#pythagorean-theorem); deleting an auxiliary right-angle vertex preserves it by the [law of cosines](geometry-and-topology.md#law-of-cosines).

## Randomized rounding

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A method turning a solution of a continuous optimization relaxation into a random feasible solution of a discrete problem. An expected objective bound can give an approximation guarantee. [Gaussian hyperplane rounding](#gaussian-hyperplane-rounding) and [Rademacher rounding for a semidefinite relaxation](convex-optimization.md#rademacher-rounding-for-a-semidefinite-relaxation) are different examples.

### Gaussian hyperplane rounding

↑ **Parent:** [Randomized rounding](#randomized-rounding)

Given a real unit-vector [Gram matrix](linear-algebra.md#gram-matrix) $Y_{ij}=\langle v_i,v_j\rangle$, draw a [standard Gaussian random vector](probability-and-statistics.md#standard-gaussian-random-vector) $Z$ and set $y_i=\operatorname{sign}\langle v_i,Z\rangle$. Each coordinate is [almost surely](convergence-of-random-variables.md#almost-sure-convergence) a sign; zero projections have [probability](probability-theory.md#probability) zero. The same random separating hyperplane is used for every coordinate, so the signs need not be [independent](random-variable.md#independent-random-variables). Their pair expectations follow the [Gaussian sign-correlation identity](probability-and-statistics.md#gaussian-sign-correlation-identity).

#### Krivine rounding scheme

↑ **Parent:** [Gaussian hyperplane rounding](#gaussian-hyperplane-rounding)

For a bipartite [elliptope](#elliptope) [matrix](vector-space.md#matrix) $X$, put $t=\log(1+\sqrt2)$ and apply $\sinh(tx)$ within the two diagonal blocks and $\sin(tx)$ across them. Matching absolute [power series](real-analysis.md#power-series) [coefficients](vector-space.md#coefficient) give a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) by [coefficient-dominated entrywise positivity](linear-algebra.md#coefficient-dominated-entrywise-positivity), while $\sinh t=1$ gives unit diagonal. [Gaussian hyperplane rounding](#gaussian-hyperplane-rounding) then turns each cross-block [correlation coefficient](variance.md#pearson-correlation-coefficient) into $(2/\pi)\arcsin(\sin(tX_{ij}))=(2t/\pi)X_{ij}$ because $t<\pi/2$. The zero diagonal blocks of the bipartite objective eliminate every other contribution.

##### Bipartite sign rounding bound

↑ **Parent:** [Krivine rounding scheme](#krivine-rounding-scheme)

For [bipartite binary quadratic optimization](#bipartite-binary-quadratic-optimization), if $v^*$ is the sign optimum and $p^*_{\rm SDP}$ its [semidefinite relaxation of binary quadratic optimization](convex-optimization.md#semidefinite-relaxation-of-binary-quadratic-optimization) value, then $c_Kp^*_{\rm SDP}\leq v^*\leq p^*_{\rm SDP}$. The upper bound follows from rank-one lifting. For the lower bound, [Krivine rounding scheme](#krivine-rounding-scheme) preprocessing followed by [Gaussian hyperplane rounding](#gaussian-hyperplane-rounding) has expected objective exactly $c_Kp^*_{\rm SDP}$, and every rounded [vector](vector-space.md#vector) is feasible. Some outcome reaches at least this [expectation](probability-theory.md#expected-value). No [independence](random-variable.md#independent-random-variables) of rounded coordinates or [positive semidefiniteness](linear-algebra.md#positive-semidefinite-matrix) of the original bipartite objective is needed.

##### Krivine rounding constant

↑ **Parent:** [Krivine rounding scheme](#krivine-rounding-scheme)

The [Krivine rounding scheme](#krivine-rounding-scheme) yields $c_K=0.56109985\ldots$ as its guaranteed objective factor. It is obtained by normalizing $\sinh t=1$, so $t=\operatorname{arsinh}(1)$ and $c_K=2t/\pi$. This proof gives a valid universal factor for the bipartite sign problem, not a proof that it is optimal.

## Quadratic optimization

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

Optimization of a [quadratic form](linear-algebra.md#quadratic-form) or quadratic-plus-linear objective over specified constraints. Convexity depends on the [matrix](vector-space.md#matrix) and feasible domain; discrete restrictions lead to [binary quadratic optimization](#binary-quadratic-optimization).

### Quadratic program

↑ **Parent:** [Quadratic optimization](#quadratic-optimization)

A [quadratic program](#quadratic-program) is an optimization problem with a quadratic objective and linear equality or inequality constraints. A positive-definite objective Hessian makes it [strictly convex](real-analysis.md#strictly-convex-function) and coercive; on a nonempty closed feasible set its minimizer exists and is unique. Such a program resolves tied Lasso knots by constraining tangent signs of currently zero [regression coefficients](linear-regression.md#regression-coefficient) while allowing unrestricted tangents for nonzero ones.

### Binary quadratic optimization

↑ **Parent:** [Quadratic optimization](#quadratic-optimization)

Optimization of a [quadratic form](linear-algebra.md#quadratic-form) over binary choices, here using signs $x_i\in\{-1,1\}$. Lifting $xx^T$ turns the objective into a [matrix trace](linear-algebra.md#matrix-trace); dropping the rank-one condition gives a [semidefinite relaxation of binary quadratic optimization](convex-optimization.md#semidefinite-relaxation-of-binary-quadratic-optimization).

#### Bipartite binary quadratic optimization

↑ **Parent:** [Binary quadratic optimization](#binary-quadratic-optimization)

For a real rectangular [matrix](vector-space.md#matrix) $S$, maximize $p^TSq$ over separate sign choices for $p$ and $q$. With $x=(p,q)$, the symmetric block [matrix](vector-space.md#matrix) $A=\tfrac12\begin{pmatrix}0&S\\S^T&0\end{pmatrix}$ satisfies $x^TAx=p^TSq$. Its zero diagonal blocks allow the [Krivine rounding scheme](#krivine-rounding-scheme) to linearize the cross-block expected objective.

## Optimal transport

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Optimal_transport)

Optimal transport minimizes the cost of moving one [probability measure](probability-theory.md#probability-measure) to another. The [Monge optimal transport problem](#monge-optimal-transport-problem) uses a [transport map](#transport-map); the [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem) allows a [transport plan](#transport-plan) that can split mass.

### c-cyclical monotonicity

↑ **Parent:** [Optimal transport](#optimal-transport)

A set of source-destination pairs has this property if every finite cyclic reassignment of destinations cannot lower its total cost. A [transport plan](#transport-plan) has the property if it is concentrated on such a set. For a general cost, this is stronger than a two-point monotonicity test.

#### Finite-cost optimal transport converse

↑ **Parent:** [C-cyclical monotonicity](#c-cyclical-monotonicity)

An optimal [transport plan](#transport-plan) of finite cost for a finite continuous cost [function](function.md) is [c-cyclically monotone](#c-cyclical-monotonicity). A strict violation at finitely many support points persists in small product neighborhoods; subtracting small normalized pieces and inserting cyclically re-paired product [measures](measure-theory.md#measure) preserves both marginals and strictly improves the finite cost. The finite-value hypothesis matters: if every competitor has infinite cost, a nonmonotone plan may still be an extended-value minimizer.

#### Strong c-monotonicity

↑ **Parent:** [C-cyclical monotonicity](#c-cyclical-monotonicity)

A [transport plan](#transport-plan) is strongly c-monotone if Borel [Kantorovich potentials](#kantorovich-potential) satisfy the displayed feasible inequality everywhere and equality almost everywhere for the plan. Extended values $-\infty$ away from the full marginal-[measure](measure-theory.md#measure) sets may be permitted. This is a potential certificate, not a strict version of every cyclic inequality. A finite continuous cost allows the [transport potential path construction](#transport-potential-path-construction).

##### Symmetric clipping proof of transport optimality

↑ **Parent:** [Strong c-monotonicity](#strong-c-monotonicity)

For a nonnegative cost, simultaneous symmetric clipping preserves feasibility of a pair of [Kantorovich potentials](#kantorovich-potential). On their equality set the clipped sums are nonnegative and increase to the cost. Their bounded integrals are fixed by the marginals, so [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) proves optimality without subtracting undefined infinite marginal integrals.

##### Transport potential path construction

↑ **Parent:** [Strong c-monotonicity](#strong-c-monotonicity)

Anchor a countable dense subset of a closed [c-cyclically monotone](#c-cyclical-monotonicity) support. Take the infimum of accumulated differences $c(x_{j+1},y_j)-c(x_j,y_j)$ along chains ending at a variable point. Cyclical monotonicity bounds this potential below on the support projection. Its cost transform gives the other potential, with equality on the support. Continuity makes both potentials [upper semicontinuous](calculus.md#upper-semicontinuity) and thus Borel.

### Monotone rearrangement

↑ **Parent:** [Optimal transport](#optimal-transport)

For an [atomless measure](measure-theory.md#non-atomic-measure) $\mu$ on $\mathbb R$ with [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $F$, the monotone transport to a target with [quantile function](probability-theory.md#quantile-function) $G^{-1}$ is $T=G^{-1}\circ F$, defined $\mu$-almost everywhere. It minimizes well-defined costs $d(x-y)$ for [convex](real-analysis.md#convex-function) continuous $d$. With atoms in the source, the common-quantile [transport plan](#transport-plan) $(F^{-1},G^{-1})_\#\mathcal U(0,1)$ remains available but need not be induced by a map.

#### One-dimensional quadratic transport uniqueness criterion

↑ **Parent:** [Monotone rearrangement](#monotone-rearrangement)

For atomless source and target probabilities with continuous strictly increasing cumulative distributions, the squared-distance optimal coupling is unique. Two-point optimality forbids crossed support pairs. This makes every pair of source and target lower-tail events nested up to null sets and forces the displayed joint distribution, which is the common-quantile coupling and is induced by $G^{-1}F$.

<h3 id="knott-smith-optimality-criterion">Knott–Smith optimality criterion</h3>

↑ **Parent:** [Optimal transport](#optimal-transport)

For [probability measures](probability-theory.md#probability-measure) on $\mathbb R^d$ with finite second [moments](probability-theory.md#moment), a [transport plan](#transport-plan) minimizes the quadratic cost exactly when it is concentrated on the graph of the [subdifferential](convex-optimization.md#subdifferential) of a [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity) [proper convex function](real-analysis.md#proper-convex-function).

#### Brenier theorem

↑ **Parent:** [Knott–Smith optimality criterion](#knott-smith-optimality-criterion)

For [probability measures](probability-theory.md#probability-measure) on $\mathbb R^d$ with finite second [moments](probability-theory.md#moment) and a source satisfying [absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures) with respect to [Lebesgue measure](measure-theory.md#lebesgue-measure), the quadratic [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem) has a unique optimal [transport plan](#transport-plan). It is induced by the [gradient](calculus.md#gradient) of a [convex function](real-analysis.md#convex-function), which also uniquely solves the [Monge optimal transport problem](#monge-optimal-transport-problem) up to a source-null set.

### Kantorovich optimal transport problem

↑ **Parent:** [Optimal transport](#optimal-transport)

The Kantorovich problem minimizes $\int c(x,y)\,d\pi(x,y)$ over [transport plans](#transport-plan) $\pi$ with [marginal distributions](probability-theory.md#marginal-distribution) $\mu,\nu$. It relaxes the [Monge optimal transport problem](#monge-optimal-transport-problem) by allowing source mass to split among destinations.

#### Transport cost function

↑ **Parent:** [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem)

The transport cost [function](function.md) assigns a cost to a unit of mass moved from $x$ to $y$. A [transport plan](#transport-plan) has total cost $\int c\,d\pi$. Costs separating as $a(x)+b(y)$ have the same well-defined total for every coupling of fixed marginals.

#### Kantorovich duality theorem

↑ **Parent:** [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem)

For [probability measures](probability-theory.md#probability-measure) defined as [Borel measures](measure-theory.md#borel-measure) on [Polish spaces](topological-analysis.md#polish-space) and a nonnegative [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity) cost, the minimum cost over [transport plans](#transport-plan) equals the supremum of $\int u\,d\mu+\int v\,d\nu$ over integrable [Kantorovich potentials](#kantorovich-potential) satisfying $u(x)+v(y)\leq c(x,y)$. The primal minimum is attained; a dual maximum needs additional assumptions. Compact metric spaces and a finite continuous cost suffice for attainment of both extrema.

##### Kantorovich duality by positive extension

↑ **Parent:** [Kantorovich duality theorem](#kantorovich-duality-theorem)

For compact metric spaces and a continuous cost, define the marginal functional $\ell(f(x)+g(y))=\int f\,dP+\int g\,dQ$. Its majorant envelope $p(h)=\inf_{s\geq h}\ell(s)$ is finite and sublinear. The dual value is $-p(-c)$. Assign that value to the cost direction and use the dominated [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) to obtain a [positive linear functional](continuous-dual-space.md#positive-linear-functional) on all continuous functions of two variables. The [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) turns it into an optimal [transport plan](#transport-plan) with the prescribed marginals.

##### Kantorovich potential

↑ **Parent:** [Kantorovich duality theorem](#kantorovich-duality-theorem)

Kantorovich potentials are the functions in the dual of the [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem). A feasible pair satisfies $u(x)+v(y)\leq c(x,y)$ and provides a lower bound $\int u\,d\mu+\int v\,d\nu$ for every [transport plan](#transport-plan). An optimal pair attaining the dual value provides an optimality certificate.

#### Transport plan

↑ **Parent:** [Kantorovich optimal transport problem](#kantorovich-optimal-transport-problem)

A transport plan is a [coupling of probability distributions](probability-and-statistics.md#coupling) $\mu,\nu$, that is, a [probability measure](probability-theory.md#probability-measure) on the product space with those [marginal distributions](probability-theory.md#marginal-distribution). Unlike a [transport map](#transport-map), it need not be concentrated on the graph of a function.

### Monge optimal transport problem

↑ **Parent:** [Optimal transport](#optimal-transport)

Given a cost $c$ and [probability measures](probability-theory.md#probability-measure) $\mu,\nu$, the Monge problem minimizes $\int c(x,T(x))\,d\mu(x)$ over measurable [transport maps](#transport-map) with [pushforward measure](measure-theory.md#pushforward-measure) $T_\#\mu=\nu$. The feasible set may be empty because a map cannot split an [atom of a measure](measure-theory.md#atom-measure-theory).

#### Transport map

↑ **Parent:** [Monge optimal transport problem](#monge-optimal-transport-problem)

A transport map from $\mu$ to $\nu$ is a [measurable function](measure-theory.md#measurable-function) $T$ satisfying $T_\#\mu=\nu$. Its graph defines the [transport plan](#transport-plan) $(\operatorname{Id},T)_\#\mu$.

##### Measure-preserving parametrization of one-dimensional transport maps

↑ **Parent:** [Transport map](#transport-map)

When source and target have continuous strictly increasing cumulative distributions, all [transport maps](#transport-map) are obtained by choosing a [Lebesgue-measure-preserving map](measure-theory.md#lebesgue-measure-preserving-map) $S$ on the unit interval. The maps $F$ and $G$ turn the two [measures](measure-theory.md#measure) into uniform [measure](measure-theory.md#measure). The choice $S=\mathrm{id}$ gives the [monotone rearrangement](#monotone-rearrangement).

## Lagrange sufficiency theorem

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

For maximizing $f$ subject to $g_i(x)\geq0$ and $h_j(x)=0$, suppose a feasible $x^*$ and multipliers $\lambda_i\geq0,\mu_j$ satisfy complementary slackness and $x^*$ globally maximizes

$$
L(x)=f(x)+\sum_i\lambda_i g_i(x)+\sum_j\mu_jh_j(x).
$$

Then $x^*$ globally maximizes $f$ on the feasible set. Convexity or concavity hypotheses are commonly used to prove the required global extremum of the Lagrangian from first-order conditions.

### Minimum squared norm under two affine constraints

↑ **Parent:** [Lagrange sufficiency theorem](#lagrange-sufficiency-theorem)

For real $a_i$ not all equal, let $S_1=\sum_i a_i$, $S_2=\sum_i a_i^2$ and $\Delta=nS_2-S_1^2>0$. The unique minimizer of $\sum_i x_i^2$ under $\sum_i x_i=1$, $\sum_i a_ix_i=0$ is $x_i^*=(S_2-S_1a_i)/\Delta$, with minimum $S_2/\Delta$. To prove sufficiency, the [optimization Lagrangian](#optimization-lagrangian) with multipliers $\lambda=S_2/\Delta$, $\mu=-S_1/\Delta$ is a sum of squares in $x_i-\lambda-\mu a_i$ plus a constant. Equivalently every feasible $x$ satisfies $\sum_i x_i^2-\sum_i(x_i^*)^2=\sum_i(x_i-x_i^*)^2$.

### Scalar multiplier certificate for a quadratic equality constraint

↑ **Parent:** [Lagrange sufficiency theorem](#lagrange-sufficiency-theorem)

For $\gamma>0$ and $c\ne0$, minimize $c^Tu+\gamma z^2$ subject to $\|u\|^2+z=R$. Adding a positive [Lagrange multiplier](#lagrange-multiplier) times the constraint gives a [positive-definite](linear-algebra.md#positive-definite-bilinear-form) quadratic [optimization Lagrangian](#optimization-lagrangian), whose minimizer is $u=-c/(2\lambda)$ and $z=-\lambda/(2\gamma)$. Feasibility is the displayed scalar equation. Its left side strictly decreases from positive infinity to negative infinity on $\lambda>0$, so it has a unique root for every real $R$. The [Lagrangian sufficiency theorem](#lagrange-sufficiency-theorem) certifies a unique global optimum on the possibly nonconvex equality surface.

## Dynamic programming

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dynamic_programming)

Dynamic programming solves a multistage optimization problem backwards by expressing each remaining-horizon value in terms of the next-stage value.

### Dynamic programming principle

↑ **Parent:** [Dynamic programming](#dynamic-programming)

An optimal value over a time interval is the supremum of immediate reward plus the conditional optimal continuation value. For a controlled state $X$ and running reward $\ell$, this reads $J(x,t)=\sup_a\mathbb E[\int_t^{t+h}\ell(X_s,a_s,s)ds+J(X_{t+h},t+h)\mid X_t=x]$, under the usual admissible concatenation and information conditions. Conditioning and concatenating strategies proves both inequalities: every strategy's continuation is bounded by the value function, while approximately optimal continuations approach that bound. For a smooth diffusion value function, [Itô formula](stochastic-calculus.md#ito-s-lemma) and the limit $h\downarrow0$ yield the [Hamilton-Jacobi-Bellman equation](#hamilton-jacobi-bellman-equation).

### Average-reward optimal policy

↑ **Parent:** [Dynamic programming](#dynamic-programming)

An average-reward optimal policy maximizes long-run expected reward per time step. In a finite recurrent [Markov chain](markov-process.md#markov-chain), a stationary policy's gain is its expected one-step reward under the stationary distribution. Initial-state effects are encoded by a bias function rather than by the gain. In a communicating finite control problem, the [average-reward Bellman equation](#average-reward-bellman-equation) certifies a policy that is optimal from every initial state.

#### Average-reward Bellman equation

↑ **Parent:** [Average-reward optimal policy](#average-reward-optimal-policy)

The gain $g$ and bounded bias $h$ in this equation give an upper bound on average reward for every policy: summing its action inequalities telescopes the bias, leaving total expected reward at most $ng+h(i)-\mathbb Eh(X_n)$. A stationary maximizing action at each state attains equality and hence the gain $g$. Policy improvement computes the current gain and bias, then switches to actions with greater reward-plus-expected-bias value.

### Control policy

↑ **Parent:** [Dynamic programming](#dynamic-programming)

A control policy selects admissible actions using only the information available at each time, possibly with randomization. General policies may depend on the whole observed history. Nonanticipation and measurability are part of admissibility in a [controlled Markov process](control-theory.md#controlled-markov-process).

#### Markov policy

↑ **Parent:** [Control policy](#control-policy)

A Markov policy uses only the current state and, in the nonstationary case, the current time. A stationary Markov policy has the form $u_t=u_*(X_t)$ for one measurable selector $u_*$. It is a restricted class of [control policies](#control-policy), whose sufficiency for an optimization problem requires the appropriate dynamic-programming hypotheses.

### Retirement threshold with multiplicative capture risk

↑ **Parent:** [Dynamic programming](#dynamic-programming)

If a successful step in action $i$ has expected reward $a_i\geq0$ and survival probability $q_i=1-p_i$, a finite-horizon retirement problem with zero wealth after capture has threshold $\max_i a_iq_i/p_i$. Above it, induction makes retirement optimal; below it, a single further step already beats retirement. The threshold does not depend on the remaining positive horizon.

### Bellman equation

↑ **Parent:** [Dynamic programming](#dynamic-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bellman_equation)

A Bellman equation is the recursive optimality relation for the [value function](#value-function) of a [dynamic programming](#dynamic-programming) problem.

#### Dynamic programming operator

↑ **Parent:** [Bellman equation](#bellman-equation)

This one-step operator combines immediate cost with optimized discounted continuation. It is monotone. For nonnegative costs, iterating it from zero produces increasing finite-horizon values bounded above by the infinite-horizon value. If a nonnegative fixed point has a minimizing measurable selector, repeated conditional expectation and dropping the nonnegative terminal value show that the corresponding stationary policy costs no more than that fixed point. Thus the infinite-horizon value, when the [Bellman equation](#bellman-equation) holds, is the least nonnegative fixed point.

#### Bellman comparison with nonnegative rewards and superunit discount

↑ **Parent:** [Bellman equation](#bellman-equation)

For nonnegative rewards, a nonnegative value satisfying the maximizing [Bellman equation](#bellman-equation) dominates every competing policy, even for $\beta\geq1$. Iterate the one-step inequality, discard the nonnegative terminal value, then apply the [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) to the accumulated reward.

#### Hamilton-Jacobi-Bellman equation

↑ **Parent:** [Bellman equation](#bellman-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamilton-Jacobi-Bellman_equation)

The Hamilton--Jacobi--Bellman equation is the continuous-time [Bellman equation](#bellman-equation). For state dynamics $\dot x=f(x,u,t)$, running cost $L(x,u,t)$ and terminal cost $\Phi(x)$, a smooth [value function](#value-function) satisfies

$$
V_t+\inf_u\{L+\nabla V\mathbin{\cdot}f\}=0,
\qquad V(x,h)=\Phi(x).
$$

##### Verification by a nonnegative control supermartingale

↑ **Parent:** [Hamilton-Jacobi-Bellman equation](#hamilton-jacobi-bellman-equation)

For a nonnegative classical solution $V$ of a finite-horizon [Hamilton-Jacobi-Bellman equation](#hamilton-jacobi-bellman-equation) with nonnegative running reward $r$, the process $V(X_t,t)+\int_0^t r(X_s,a_s)ds$ is a local [supermartingale](martingale.md#supermartingale) under every admissible control. The [Itô formula](stochastic-calculus.md#ito-s-lemma) gives nonpositive drift because the chosen control cannot exceed the supremum in the equation. Stop where the [stochastic integral](stochastic-calculus.md#stochastic-integral) becomes a true [martingale](martingale.md), take expectations and apply the [Fatou lemma](measure-theory.md#fatou-s-lemma). Nonnegativity prevents loss of a lower bound when removing the stops, giving the verification upper bound. A maximizing control attains the bound when its stopped reward processes are [uniformly integrable](convergence-of-random-variables.md#uniform-integrability).

##### Linear-quadratic optimal control

↑ **Parent:** [Hamilton-Jacobi-Bellman equation](#hamilton-jacobi-bellman-equation)

A linear-quadratic optimal-control problem has [linear](vector-space.md#linearity) state dynamics and running and terminal costs defined by [quadratic forms](linear-algebra.md#quadratic-form). Its value function is quadratic in the state, the optimal feedback is linear, and its coefficient obeys a [Riccati equation](analysis.md#riccati-equation).

###### Discrete Riccati recurrence

↑ **Parent:** [Linear-quadratic optimal control](#linear-quadratic-optimal-control)

A backward scalar or matrix recurrence for the quadratic coefficients in a value function for a [linear-quadratic optimal control](#linear-quadratic-optimal-control) problem. It results from completing the control square in the [Bellman equation](#bellman-equation). Multiplicative noise modifies the quadratic coefficients through its second moments.

### Value function

↑ **Parent:** [Dynamic programming](#dynamic-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Value_function)

A value function assigns each state and time the best objective attainable from that state over the remaining decisions.

#### Non-vertical supporting hyperplane of a value function

↑ **Parent:** [Value function](#value-function)

At a point where $\phi(b)$ is finite, this is an affine plane supporting the [epigraph](calculus-of-variations.md#epigraph) from below: $\phi(u)\geq\phi(b)+\lambda^T(u-b)$ for every $u$. A nonzero coefficient of the vertical coordinate permits normalization to the displayed graph form. For a constrained [value function](#value-function), the slope is exactly an attained multiplier in the [Strong Lagrangian property](#strong-lagrangian-property). When the [value function](#value-function) is differentiable at an interior point of its finite domain, a supporting slope equals its [gradient](calculus.md#gradient): apply the supporting inequality along both positive and negative multiples of each coordinate direction and take limits.

### Bayesian box search problem

↑ **Parent:** [Dynamic programming](#dynamic-programming)

A hidden object lies in box $i$ with posterior probability $p_i$. Searching box $i$ costs $c_i$ and, conditional on the object being there, detects it with probability $\alpha_i$. After an unsuccessful search of box $i$, [Bayes' theorem](probability-theory.md#bayes-theorem) updates the probabilities to

$$
p_i^{(i)}=\frac{(1-\alpha_i)p_i}{1-\alpha_ip_i},
\qquad
p_j^{(i)}=\frac{p_j}{1-\alpha_ip_i}\quad(j\ne i).
$$

#### Optimal index for Bayesian box search

↑ **Parent:** [Bayesian box search problem](#bayesian-box-search-problem)

When search continues until discovery, expected search cost is minimized by searching at each step a box maximizing $\alpha_i p_i/c_i$. An adjacent-interchange argument compares two searches: placing $i$ before $j$ costs less exactly when $\alpha_ip_i/c_i\geq\alpha_jp_j/c_j$.

#### Rewarded Bayesian box search Bellman equation

↑ **Parent:** [Bayesian box search problem](#bayesian-box-search-problem)

If discovery in box $i$ earns reward $R_i$ and stopping earns zero, the [Bellman equation](#bellman-equation) is

$$
V(p)=\max\left\{0,
\max_i\left[-c_i+\alpha_ip_iR_i
+(1-\alpha_ip_i)V(p^{(i)})\right]\right\}.
$$

If $\sum_i c_i/(\alpha_iR_i)<1$, every posterior state has some $i$ with $\alpha_ip_iR_i>c_i$, so stopping is never optimal.

<h2 id="newton-s-method-in-optimization">Newton's method in optimization</h2>

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton's_method_in_optimization)

Newton's method for minimizing a twice differentiable function uses

$$
x_{k+1}=x_k-[\nabla^2f(x_k)]^{-1}\nabla f(x_k).
$$

<h3 id="quadratic-convergence-bound-for-newton-s-method">Quadratic convergence bound for Newton's method</h3>

↑ **Parent:** [Newton's method in optimization](#newton-s-method-in-optimization)

If $\nabla^2f\succeq mI$ and the Hessian is $M$-Lipschitz near a minimizer $x^*$, then

$$
\|x_{k+1}-x^*\|\leq\frac{M}{2m}\|x_k-x^*\|^2.
$$

Thus a sufficiently close initial point has an error exponent that doubles at each iteration.

## Karush-Kuhn-Tucker conditions

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karush-Kuhn-Tucker_conditions)

For differentiable inequality constraints $g_i(x)\leq0$, a regular local minimum has multipliers $\lambda_i\geq0$ satisfying

$$
\nabla f+\sum_i\lambda_i\nabla g_i=0,
\qquad
\lambda_i g_i=0.
$$

For a convex problem under a suitable constraint qualification, these conditions are sufficient for global optimality.

### Active-set transition in capped resource allocation

↑ **Parent:** [Karush-Kuhn-Tucker conditions](#karush-kuhn-tucker-conditions)

In a convex resource-allocation problem, tightening an upper bound can change its multiplier from zero to positive. The optimum then moves from a point where only the total-resource constraint is active to the intersection where both constraints are active.

## Convex optimization

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

[This section is present in another page, follow this link to view it.](convex-optimization.md)

## Lagrange multiplier

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange_multiplier)

At a regular constrained extremum of $f$ subject to $g=0$, the gradients satisfy

$$
\nabla f=\lambda\nabla g.
$$

### Maximum box volume in an ellipsoid

↑ **Parent:** [Lagrange multiplier](#lagrange-multiplier)

For an axis-aligned box, maximize $xyz$ subject to $x^2/a^2+y^2/b^2+z^2/c^2=1$. The [Lagrange multiplier](#lagrange-multiplier) equations imply $x^2/a^2=y^2/b^2=z^2/c^2=1/3$. Boundary boxes have zero volume, so this gives the maximum. Arbitrary orientation cannot improve it: averaging the ellipsoid inequality over the eight vertices gives a sum of three squared transformed half-edge lengths at most one; the determinant bound and arithmetic-geometric mean bound their product by $1/(3\sqrt3)$.

### Minimum-area closed cylinder at fixed volume

↑ **Parent:** [Lagrange multiplier](#lagrange-multiplier)

For radius $r>0$ and height $h>0$, volume is $\pi r^2h$ and area including both ends is $2\pi r^2+2\pi rh$. The [Lagrange multiplier](#lagrange-multiplier) equations give $h=2r$. Substituting the constraint gives the one-variable function $2\pi r^2+2V/r$, which tends to infinity at both ends and has its only stationary point at $r^3=V/(2\pi)$. This proves the stationary cylinder is the unique global minimizer.

### Envelope theorem

↑ **Parent:** [Lagrange multiplier](#lagrange-multiplier)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Envelope_theorem)

For a smooth constrained maximum $\phi(b)=f(\bar x(b))$ subject to $g(\bar x(b))=b$, suppose smooth optimizers and multipliers satisfy $\nabla f(\bar x)=Dg(\bar x)^T\lambda$. Differentiating the constraint gives $Dg(\bar x)D_b\bar x=I$, and the chain rule gives $D_b\phi=\lambda^T$. Thus a [Lagrange multiplier](#lagrange-multiplier) measures the marginal value of relaxing its corresponding constraint. A global supporting [Lagrangian duality](#lagrangian-duality) representation implies the needed stationarity, but local stationarity and smoothness alone suffice for this derivative identity.

### Optimization Lagrangian

↑ **Parent:** [Lagrange multiplier](#lagrange-multiplier)

For a [minimization problem](#minimization-problem) with $g_i(u)\leq0$ and $h_j(u)=0$, the optimization Lagrangian is $L=f+\sum_i\lambda_i g_i+\sum_j\mu_jh_j$ with $\lambda_i\geq0$ and unrestricted equality [Lagrange multipliers](#lagrange-multiplier). Its infimum over the original variable domain gives a dual lower bound. For a [maximization problem](#maximization-problem), use $L=f-\sum_i\lambda_i g_i-\sum_j\mu_jh_j$ to obtain upper bounds. The [Lagrangian sufficiency theorem](#lagrange-sufficiency-theorem) combines a global extremum of this function with feasibility and [complementary slackness](#complementary-slackness). This is distinct from a [Lagrangian](calculus-of-variations.md#lagrangian) density in variational physics.

### Derivative of a constrained value function

↑ **Parent:** [Lagrange multiplier](#lagrange-multiplier)

For

$$
\phi(b)=\inf\{f(x):g(x)=b\},
$$

suppose the optimizer and multiplier vary smoothly and use $L=f-\lambda(g-b)$. Differentiating the optimum value and using stationarity gives

$$
\phi'(b)=\lambda(b).
$$

### Weighted open-box minimization

↑ **Parent:** [Lagrange multiplier](#lagrange-multiplier)

For a topless rectangular box with dimensions $x,y,z$, volume $V$, and weighted face cost

$$
A=axy+bxz+cyz,
$$

an interior optimum equalizes the three terms:

$$
axy=bxz=cyz.
$$

The same result and global minimality follow from the arithmetic-geometric mean inequality.

## Arithmetic-geometric mean inequality

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arithmetic-geometric_mean_inequality)

For nonnegative $a_1,\ldots,a_n$,

$$
\frac{a_1+\cdots+a_n}{n}\geq(a_1\cdots a_n)^{1/n},
$$

with equality exactly when all the $a_i$ are equal.

## Linear programming

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_programming)

Linear programming optimizes a [linear function](vector-space.md#linear-function) subject to finitely many linear equalities and inequalities.

### Karmarkar standard form

↑ **Parent:** [Linear programming](#linear-programming)

This form of [linear programming](#linear-programming) additionally has the uniform [vector](vector-space.md#vector) as a strictly positive [feasible point](#feasible-point) and known optimum zero. A [homogeneous self-dual embedding of a linear program](convex-optimization.md#homogeneous-self-dual-embedding-of-a-linear-program), followed by elimination of unrestricted [Lagrange multipliers](#lagrange-multiplier) and normalization by the sum of nonnegative coordinates, yields this form without presupposing feasibility of the original program. The known start and optimum support projective [interior-point methods](convex-optimization.md#interior-point-method). Polynomial bit-complexity statements additionally require finite rational input encoding; bounded arbitrary real coefficients alone do not provide it.

### Surplus variable

↑ **Parent:** [Linear programming](#linear-programming)

A surplus variable converts a lower-bound inequality $a^Tx\ge b$ into $a^Tx-z=b$, with $z\ge0$. This is the lower-bound counterpart of a [slack variable](#slack-variable). When the original coefficients, right-hand side and decision variables are integer, the surplus variable is integer as well; that fact permits it to appear in an all-integer [Gomory fractional cut](#gomory-fractional-cut) row.

### Optimal face of a linear program

↑ **Parent:** [Linear programming](#linear-programming)

The set of minimizers of a linear objective on a [linear polyhedron](#linear-polyhedron). It is a face: if a strict convex combination of two feasible points minimizes the objective, both points must also minimize it. Hence an [extreme point](#extreme-point) of an optimal face is an extreme point of the original polyhedron. Successively minimizing further linear objectives restricts to nested faces, whose vertices remain original vertices. This preserves uniform rational denominator bounds in exact feasibility-oracle optimization.

### Rational feasibility certificate for integer inequalities

↑ **Parent:** [Linear programming](#linear-programming)

A nonempty [linear polyhedron](#linear-polyhedron) with integer inequality coefficients and right sides bounded by $U\geq1$ contains a point $x_i=p_i/q_i$ with the displayed bounds. Intersect with an orthant containing a feasible point. Moving along directions annihilating the active constraints, until another constraint becomes active, produces a vertex: the orthant prevents a whole nontrivial line from remaining feasible. At that vertex, choose $n$ independent active inequalities, including coordinate constraints as necessary. [Cramer's rule](linear-algebra.md#cramer-s-rule) and the [Hadamard determinant inequality](linear-algebra.md#hadamard-determinant-inequality) bound both determinants by $n^{n/2}U^n\leq(nU)^n$. The resulting rational witness has polynomial binary length and is verifiable in [polynomial time](computer-science.md#polynomial-time), proving that integer linear feasibility is in [NP](computer-science.md#np-complexity).

### Ellipsoid method

↑ **Parent:** [Linear programming](#linear-programming)

The [ellipsoid method](#ellipsoid-method) repeatedly asks a [separation oracle](convex-optimization.md#separation-oracle) about the center of a containing ellipsoid and replaces that ellipsoid by a smaller one containing its intersection with a separating half-space. The volume decreases by a dimension-dependent factor at each iteration. For rational polyhedra, the exact feasibility theorem has polynomial bit complexity in the dimension and coefficient encoding bounds when separation is [polynomial time](computer-science.md#polynomial-time). It includes lower-dimensional feasible sets through rational precision bounds or suitable relaxations; one must not declare infeasibility just because the original feasible set has zero volume.

#### Feasible-point box bound for a polyhedron with lines

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

A nonempty [linear polyhedron](#linear-polyhedron) can have no extreme point. Intersect it with an orthant containing one feasible point, and minimize the sum of the signed coordinates there. The relevant sublevel sets are compact, so the minimum face has an extreme point, which is also extreme in the orthant intersection. The added signed-coordinate rows are integer rows with entries at most one. The [integer-matrix vertex coordinate bound](#integer-matrix-vertex-coordinate-bound) gives $R=n!\max(1,U)^n$. This supplies a bounded feasibility search even when the original polyhedron contains lines.

#### Full-dimensional relaxation of integer inequalities

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

For an integer [linear polyhedron](#linear-polyhedron) $P=\{x\in\mathbb R^n:Ax\geq b\}$ with coefficients bounded by $U\geq1$, put $D=[(n+1)U]^{n+1}$ and $0<\varepsilon<1/D$. If $x_0\in P$, every $h$ with $\|h\|_2\leq\varepsilon/(nU)$ satisfies $A_i h\geq-\sqrt n U\|h\|_2\geq-\varepsilon$. Thus $P_\varepsilon$ contains a positive-radius [Euclidean ball](functional-analysis.md#euclidean-ball) and is a [full-dimensional linear polyhedron](#full-dimensional-linear-polyhedron). If $P$ is empty, the [normalized integer Farkas infeasibility gap](convex-optimization.md#normalized-integer-farkas-infeasibility-gap) gives $\lambda\geq0$, $A^T\lambda=0$, $\mathbf1^T\lambda=1$ and $b^T\lambda\geq1/D$. A point of $P_\varepsilon$ would give $0=\lambda^TAx\geq b^T\lambda-\varepsilon>0$, a contradiction. Consequently this relaxation preserves emptiness and supplies the inner-volume bound needed by the [ellipsoid method](#ellipsoid-method), even when $P$ has empty interior.

#### Exact linear optimization from a feasibility oracle

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

A [polynomial-time algorithm](computer-science.md#polynomial-time-algorithm) for integer linear feasibility gives exact rational [linear programming](#linear-programming) optimization. Rational vertex bounds give a polynomial-bit bound on every finite optimal value and its denominator. An objective threshold below that bound detects unboundedness after feasibility is established. Binary search with the additional inequality $c^Tx\leq t$ localizes the finite optimum to an interval containing a unique rational of bounded denominator; [continued fractions](number-theory.md#continued-fraction) recover it exactly. A feasible optimizer can then be found by successive coordinate minimizations on a bounded optimal face. These produce faces of one fixed rational polytope, so one uniform vertex-denominator bound works throughout, avoiding exponential growth of precision requirements.

#### Central-cut ellipsoid volume bound

↑ **Parent:** [Ellipsoid method](#ellipsoid-method)

For $n\geq2$, the standard ellipsoid covering a centrally cut half of the unit ball has center $e_1/(n+1)$ and shape matrix $D'=\frac{n^2}{n^2-1}(I-\frac2{n+1}e_1e_1^T)$. Its eigenvalues are $n^2/(n+1)^2$ along $e_1$ and $n^2/(n^2-1)$ in the other directions. Hence its volume ratio is $R=\frac n{n+1}(\frac{n^2}{n^2-1})^{(n-1)/2}$. Using $\log(1-a)<-a$ and $\log(1+b)<b$ gives $\log R<-1/(2(n+1))$. Affine changes of coordinates preserve the volume ratio. The resulting geometric convergence underlies the [ellipsoid method](#ellipsoid-method); exact rational feasibility additionally needs input-dependent size, precision and lower-dimensional feasibility bounds.

### Maximum feasible subsystem

↑ **Parent:** [Linear programming](#linear-programming)

Given finitely encoded linear inequalities, a [maximum feasible subsystem](#maximum-feasible-subsystem) is a largest collection that can be simultaneously satisfied. Its decision version asks whether some $k$ inequalities admit a common solution. This is [NP-complete](computer-science.md#np-completeness), despite [polynomial time](computer-science.md#polynomial-time) feasibility testing for each fixed collection. For a graph, use nonnegative variables $x_v$, constraints $x_v\geq1$ for vertices, and $M>|V|$ copies of $x_u+x_v\leq1$ for each edge. A subsystem of size $M|E|+k$ must retain a copy of every edge constraint and at least $k$ vertex constraints; those vertices form an [independent set](graph-theory.md#independent-set-graph-theory). Conversely an [independent set](graph-theory.md#independent-set-graph-theory) of size $k$ supplies such a feasible subsystem by its indicator vector.

### Linear polyhedron

↑ **Parent:** [Linear programming](#linear-programming)

A linear polyhedron is an intersection of finitely many closed affine half-spaces in finite-dimensional real space. It may be empty, unbounded, or lower-dimensional. This usage differs from a three-dimensional geometric [polyhedron](geometry-and-topology.md#polyhedron). The [strict separation of disjoint linear polyhedra](#strict-separation-of-disjoint-linear-polyhedra) follows from [linear programming duality](#linear-programming-duality).

#### Full-dimensional linear polyhedron

↑ **Parent:** [Linear polyhedron](#linear-polyhedron)

A [linear polyhedron](#linear-polyhedron) in $\mathbb R^n$ is full-dimensional when its [affine hull](vector-space.md#affine-hull) is all of $\mathbb R^n$. Equivalently, it contains an open [Euclidean ball](functional-analysis.md#euclidean-ball). An open [Euclidean ball](functional-analysis.md#euclidean-ball) spans the ambient space. Conversely, a full-dimensional [convex set](#convex-set) contains $n+1$ affinely independent points; their [convex hull](#convex-hull) is a simplex with nonempty interior, so the set contains an open [Euclidean ball](functional-analysis.md#euclidean-ball).

#### Active constraint

↑ **Parent:** [Linear polyhedron](#linear-polyhedron)

An inequality constraint which holds with equality at the point under consideration. For $Ax\geq b$, a direction annihilating every active row permits sufficiently small feasible moves of either sign. If the active rows have rank $n$, their common solution is a [basic feasible solution](#basic-feasible-solution); the independent equalities uniquely determine it.

##### Integer-matrix vertex coordinate bound

↑ **Parent:** [Active constraint](#active-constraint)

At an [extreme point](#extreme-point) of $\{x:Ax\ge b\}$, the active rows span the ambient dimension: otherwise a nonzero direction orthogonal to all active rows permits small feasible moves of both signs. Select $n$ independent active rows to form an integer matrix $B$. Its nonzero determinant has absolute value at least one. [Cramer's rule](linear-algebra.md#cramer-s-rule) and the determinant expansion bound each coordinate by $n!U^n$, where $U$ bounds the entries of $A$ and $b$. The vector $b$ may be real; only the denominator matrix needs to be integer.

#### Strict separation of disjoint linear polyhedra

↑ **Parent:** [Linear polyhedron](#linear-polyhedron)

Nonempty disjoint [linear polyhedra](#linear-polyhedron) $P=\{x:Ax\leq b\}$ and $Q=\{y:Cy\leq d\}$ admit $h$ with a strictly positive separation gap. A phase-I [linear program](#linear-programming) minimizing common constraint violation has positive attained optimum. Its [Lagrangian dual problem](#lagrangian-dual-problem) gives nonnegative $\lambda,\mu$ with $A^T\lambda+C^T\mu=0$ and $\lambda^Tb+\mu^Td<0$. Then $h=A^T\lambda$ satisfies $h^Tx\leq\lambda^Tb<-\mu^Td\leq h^Ty$. The polyhedral hypothesis matters; arbitrary disjoint closed convex sets need not have a positive separation gap.

### Slack variable

↑ **Parent:** [Linear programming](#linear-programming)

A slack variable turns an inequality constraint $a^Tx\le b$ into the equality $a^Tx+s=b$ with $s\ge0$. Its value measures the unused amount of the constraint. In the [simplex algorithm](numerical-analysis.md#simplex-algorithm), slack variables often supply the initial [basic feasible solution](#basic-feasible-solution).

### Bernstein linear programming hierarchy for polynomial minimization

↑ **Parent:** [Linear programming](#linear-programming)

For $f$ of degree $d$ and $n\ge\max(1,d)$, compute its degree-$n$ [Bernstein basis](functional-analysis.md#bernstein-basis) coefficients and solve $\max\lambda$ subject to $\lambda\le \beta_{k,n}$, $0\le k\le n$. This is a linear program with $n+1$ inequalities. The coefficients form a convex-combination enclosure of the polynomial values, so $v_n\le\min f$. [Degree elevation of Bernstein coefficients](functional-analysis.md#degree-elevation-of-bernstein-coefficients) makes the bounds monotone. For every $\epsilon>0$, the polynomial $f-(\min f-\epsilon)$ is strictly positive, so [positive Bernstein coefficients for a strictly positive polynomial](functional-analysis.md#positive-bernstein-coefficients-for-a-strictly-positive-polynomial) gives an eventual feasible bound $\min f-\epsilon$. Hence $v_n$ converges to the true minimum. Earlier indices $n<d$ can use a one-inequality program at any common coefficient-based lower bound, preserving the stated constraint count for every positive index.

### Basic feasible solution

↑ **Parent:** [Linear programming](#linear-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Basic_feasible_solution)

For $Ax=b$, $x\geq0$, a feasible vector $x$ is basic when the columns $A_i$ indexed by its positive coordinates are linearly independent. Equivalently, enlarge those columns to a basis, set every nonbasic coordinate to zero, and solve the resulting square system.

#### Degeneracy in linear programming

↑ **Parent:** [Basic feasible solution](#basic-feasible-solution)

A [basic feasible solution](#basic-feasible-solution) is degenerate when one or more of its basic variables is zero. A [simplex algorithm](numerical-analysis.md#simplex-algorithm) pivot may then change the basis without moving the feasible point or changing the objective. Assignment networks force many zero-flow basic tree arcs.

#### Basic solution

↑ **Parent:** [Basic feasible solution](#basic-feasible-solution)

For a full-row-rank system $Ax=b$ with $m$ rows, choose $m$ linearly independent columns, set all remaining variables to zero, and solve the resulting square system. The resulting vector is a basic solution; it is feasible when it also satisfies the required nonnegativity constraints.

#### Fundamental theorem of linear programming

↑ **Parent:** [Basic feasible solution](#basic-feasible-solution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_of_linear_programming)

If a linear program has an optimal solution, it has an optimal [basic feasible solution](#basic-feasible-solution). Choose an optimum with minimal positive support. A dependence among its active columns gives a feasible two-sided perturbation; optimality makes its objective slope zero, and moving until one coordinate vanishes contradicts minimality.

### Linear-fractional programming

↑ **Parent:** [Linear programming](#linear-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear-fractional_programming)

Linear-fractional programming optimizes a ratio $c^Tx/d^Tx$ over a polyhedron on which the denominator is positive.

#### Charnes-Cooper transformation

↑ **Parent:** [Linear-fractional programming](#linear-fractional-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Charnes-Cooper_transformation)

For $d^Tx>0$, set

$$
y=\frac{x}{d^Tx},
\qquad
t=\frac1{d^Tx}.
$$

Then $d^Ty=1$, and $Ax=b$ becomes $Ay=bt$, turning a linear-fractional program into a linear program with objective $c^Ty$.

### Linear programming duality

↑ **Parent:** [Linear programming](#linear-programming)

Every linear maximization program has a dual minimization program whose feasible objective values bound the primal values.

#### Dual feasibility

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

For minimization with constraints $Ax=b$, $x\geq0$, a dual-feasible vector $y$ obeys $A^Ty\leq c$, so $b^Ty$ is a lower bound on every primal-feasible objective value. For a [simplex dictionary](numerical-analysis.md#simplex-dictionary) with basis matrix $B$, the associated vector is $y^T=c_B^TB^{-1}$. Its basic reduced costs are zero and its nonbasic reduced costs are $c_N^T-c_B^TB^{-1}A_N$. Thus nonnegative [reduced costs](#reduced-cost) are exactly dual feasibility in this minimization convention; basic primal values may still be negative, as in the [dual simplex algorithm](numerical-analysis.md#dual-simplex-algorithm).

#### Dual of a maximum of affine functions

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

Minimizing $\max_i(a_i^Tx+b_i)$ over unrestricted $x$ is a [linear program](#linear-programming) after introducing an [epigraph](calculus-of-variations.md#epigraph) variable $t$ and inequalities $a_i^Tx+b_i\leq t$. Its [optimization Lagrangian](#optimization-lagrangian) has finite infimum over $x,t$ exactly when the nonnegative multipliers sum to one and their weighted slopes sum to zero. The displayed [Lagrangian dual problem](#lagrangian-dual-problem) maximizes the resulting constant lower bound. It identifies the role of a zero-slope [convex combination](#convex-combination) of the affine functions.

#### Lagrangian dual problem

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

For a minimization problem with inequalities $g_i(x)\leq0$, the [Lagrangian](calculus-of-variations.md#lagrangian) is $L(x,\lambda)=f(x)+\sum_i\lambda_i g_i(x)$ with $\lambda_i\geq0$. The Lagrangian dual maximizes the concave dual function $q(\lambda)=\inf_xL(x,\lambda)$.

##### Lagrange dual function

↑ **Parent:** [Lagrangian dual problem](#lagrangian-dual-problem)

The [Lagrange dual function](#lagrange-dual-function) is the infimum of a [Lagrangian](calculus-of-variations.md#lagrangian) over its primal variables. It is concave in the multipliers, even before convexity of the primal problem is assumed. Maximizing it over sign-compatible multipliers gives a lower bound on a minimization problem by [weak duality](#weak-duality); appropriate convex qualifications give [strong duality](#strong-duality).

##### Lagrangian relaxation

↑ **Parent:** [Lagrangian dual problem](#lagrangian-dual-problem)

A Lagrangian relaxation moves selected constraints into the objective with appropriately signed [Lagrange multipliers](#lagrange-multiplier). Maximizing the relaxed objective over a larger easy set gives an upper bound for a constrained maximization problem. Optimizing that bound need not solve the original integer problem.

###### Lagrangian knapsack bound

↑ **Parent:** [Lagrangian relaxation](#lagrangian-relaxation)

For binary [knapsack optimization](#0-1-knapsack-problem), $U(\lambda)$ is an upper bound for every $\lambda\geq0$. Its minimum is computable from the finitely many profit-to-weight breakpoints and agrees with the [fractional knapsack problem](#fractional-knapsack-problem) optimum. Zero-weight positive-profit terms are added independently.

#### Dual linear program

↑ **Parent:** [Linear programming duality](#linear-programming-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_linear_program)

For a primal maximization problem $Ax\leq b$, $x\geq0$, the dual minimizes $b^Ty$ subject to $A^Ty\geq c$, $y\geq0$.

##### Dual variable

↑ **Parent:** [Dual linear program](#dual-linear-program)

A [dual variable](#dual-variable) is a multiplier associated with a primal constraint in a [dual linear program](#dual-linear-program). In a minimization [linear program](#linear-programming) with equality constraints $Ax=b$ and nonnegative primal variables, the [Lagrangian](calculus-of-variations.md#lagrangian) $c^Tx+y^T(b-Ax)$ yields the dual objective $b^Ty$ and inequalities $A^Ty\le c$; the equality-constraint multipliers $y$ are unrestricted in sign. For a [transportation problem](#transportation-problem), row and column [dual variables](#dual-variable) give potentials $u_i,v_j$ satisfying $u_i+v_j\le c_{ij}$. [Complementary slackness](#complementary-slackness) makes occupied routes attain equality.

#### Dual of a minimization linear program in inequality form

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

The dual pair

$$
\min\{c^Tx:Ax\geq b,\ x\geq0\}
\quad\hbox{and}\quad
\max\{b^Ty:A^Ty\leq c,\ y\geq0\}
$$

satisfies weak duality because $b^Ty\leq y^TAx=x^TA^Ty\leq c^Tx$ for every feasible pair.

#### Weak duality

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

Every feasible dual objective value bounds every feasible primal objective value.

##### Linear programming optimality certificate

↑ **Parent:** [Weak duality](#weak-duality)

For the [linear program](#linear-programming) maximizing $c^Tx$ with $Ax\le b$, $x\ge0$, a vector $y\ge0$ with $A^Ty\ge c$ proves $c^Tx\le y^Tb$ for every feasible $x$. If a feasible $x$ attains that bound, it is optimal. This is [weak duality](#weak-duality) written as a directly checkable certificate; adding nonnegative multiples of constraints suffices to verify it. The equivalent reversed-inequality certificate applies to a minimization program.

##### Strong duality

↑ **Parent:** [Weak duality](#weak-duality)

Strong duality means that the primal and dual optimal values are equal. It holds for every feasible bounded [linear program](#linear-programming) and for broad classes of [convex optimization](convex-optimization.md) problems under a constraint qualification.

###### Convex perturbation function

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

If $p$ is finite convex near zero, $p'(0;d)=\max_{y\in\partial p(0)}\langle y,d\rangle$. A singleton [subdifferential](convex-optimization.md#subdifferential) gives differentiability and a first-order expansion. For an upper-bound constraint relaxed by $z$, the derivative equals the negative of the nonnegative [Lagrange multiplier](#lagrange-multiplier); relaxing the bound can decrease the minimum value.

<h6 id="slater-s-condition">Slater's condition</h6>

↑ **Parent:** [Strong duality](#strong-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slater's_condition)

The Slater condition requires a feasible point at which every nonlinear convex inequality is strict and every affine equality holds. For a convex problem it implies [strong duality](#strong-duality) and attainment of the dual optimum under standard finiteness assumptions.

###### Exact maximum-violation penalty

↑ **Parent:** [Strong duality](#strong-duality)

An exact maximum-violation penalty replaces inequalities $g_i(x)\leq0$ by the unconstrained objective $f(x)+M\max(0,g_1(x),\ldots,g_m(x))$. If an optimal dual multiplier is $\lambda^*$, every $M>\lVert\lambda^*\rVert_1$ makes every penalized minimizer feasible and optimal.

#### Complementary slackness

↑ **Parent:** [Linear programming duality](#linear-programming-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complementary_slackness)

At a primal-dual optimum, each positive variable corresponds to a tight dual constraint and conversely for positive dual variables.

#### Transportation problem

↑ **Parent:** [Linear programming duality](#linear-programming-duality)

The transportation problem minimizes linear shipping cost while matching prescribed row supplies and column demands.

This is the finite discrete [optimal transport](#optimal-transport) problem with prescribed supply and demand marginals.

##### Production costs in a transportation problem

↑ **Parent:** [Transportation problem](#transportation-problem)

When factory $i$ incurs unit production cost $p_i$ only on goods actually shipped, add that cost to every real shipping destination in its row. Unused capacity incurs no production cost; a dummy unused-capacity column therefore keeps zero cost rather than receiving $p_i$. This changes the optimal factory utilization when capacity exceeds total demand. [Transportation dual certificate with capacity inequalities](#transportation-dual-certificate-with-capacity-inequalities) proves optimality without assuming every factory must produce at full capacity.

##### Transportation dual potentials

↑ **Parent:** [Transportation problem](#transportation-problem)

Row and column potentials satisfying the displayed inequalities give a lower bound on the cost of every feasible shipment matrix: $\sum_{ij}c_{ij}x_{ij}\geq\sum_i u_i s_i+\sum_jv_j d_j$, since row sums are supplies $s_i$ and column sums are demands $d_j$. The [reduced costs](#reduced-cost) are $c_{ij}-u_i-v_j$. A feasible matrix using only zero-reduced-cost cells attains the lower bound, proving optimality by [weak duality](#weak-duality). The [transportation simplex algorithm](#transportation-simplex-algorithm) sets these potentials by equality on a [transportation spanning tree](#transportation-spanning-tree), and enters a negative-reduced-cost cell if one exists.

###### Transportation dual certificate with capacity inequalities

↑ **Parent:** [Transportation dual potentials](#transportation-dual-potentials)

For shipments $x_{ij}\geq0$ with factory row sums at most capacities $s_i$ and shop column sums exactly demands $d_j$, the displayed dual potentials give $\sum c_{ij}x_{ij}\geq\sum_i u_i s_i+\sum_jv_jd_j$. The sign $u_i\leq0$ ensures $u_i\sum_jx_{ij}\geq u_i s_i$. Equality proves optimality. It occurs when every used cell is tight and every row with spare capacity has $u_i=0$, the relevant [complementary slackness](#complementary-slackness) conditions. A dummy demand column with zero costs converts unused capacity into a balanced [transportation problem](#transportation-problem).

##### Assignment problem

↑ **Parent:** [Transportation problem](#transportation-problem)

The assignment problem chooses a one-to-one pairing of jobs and agents minimizing their total cost. Its [minimum-cost flow](graph-theory.md#minimum-cost-flow-problem) formulation puts unit supplies on job vertices and unit demands on agent vertices of a [bipartite graph](graph-theory.md#bipartite-graph). Integral feasible flows are [perfect matchings](graph-theory.md#perfect-matching).

###### Assignment lower bound from independent task minima

↑ **Parent:** [Assignment problem](#assignment-problem)

For a partial [assignment problem](#assignment-problem), add its fixed cost to the sum, over remaining tasks, of each task's cheapest available machine cost. This is a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) because it relaxes the requirement that different tasks use distinct machines. It is an admissible bound for [branch and bound](#branch-and-bound), even though the minimizing choices may assign the same machine repeatedly.

// Target: mathematical-optimization.bigb

###### Hungarian algorithm

↑ **Parent:** [Assignment problem](#assignment-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hungarian_algorithm)

The Hungarian algorithm maintains feasible [assignment dual potentials](#assignment-dual-potentials) and a matching of equality edges. If the alternating search cannot augment, adjust reachable job and agent potentials by the smallest [reduced cost](#reduced-cost) leaving the search set. This preserves feasibility and existing matching equalities while exposing a new equality edge. A resulting [perfect matching](graph-theory.md#perfect-matching) attains the dual lower bound.

###### Assignment dual potentials

↑ **Parent:** [Assignment problem](#assignment-problem)

These feasible potentials give the lower bound $\sum_i\lambda_i-\sum_j\mu_j$ on every assignment cost. An assignment using only equality edges attains this bound and is optimal by [weak duality](#weak-duality) and [complementary slackness](#complementary-slackness).

##### Transportation polytope

↑ **Parent:** [Transportation problem](#transportation-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transportation_polytope)

The transportation polytope is the set of nonnegative matrices with fixed row and column sums.

###### Transportation spanning tree

↑ **Parent:** [Transportation polytope](#transportation-polytope)

The positive cells of a nondegenerate transportation basis form a spanning tree in the bipartite graph of supply and demand vertices.

##### Transportation simplex algorithm

↑ **Parent:** [Transportation problem](#transportation-problem)

The transportation simplex computes row and column potentials, enters a negative-reduced-cost cell, and pivots around its induced alternating cycle.

###### Northwest corner method

↑ **Parent:** [Transportation simplex algorithm](#transportation-simplex-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Northwest_corner_method)

The northwest-corner method repeatedly allocates the smaller remaining supply and demand in the current top-left cell to construct an initial transportation basis.

###### Reduced cost

↑ **Parent:** [Transportation simplex algorithm](#transportation-simplex-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_cost)

For transportation potentials, the reduced cost is $\bar c_{ij}=c_{ij}-u_i-v_j$; a negative value identifies an improving entering cell.

###### Cycle pivot

↑ **Parent:** [Transportation simplex algorithm](#transportation-simplex-algorithm)

Adding a nonbasic edge to a transportation tree creates one cycle; alternating equal additions and subtractions around it preserves every row and column sum.

##### Integrality of the transportation problem

↑ **Parent:** [Transportation problem](#transportation-problem)

Integer supplies and demands admit an integer optimum because an integer initial basis and every cycle pivot remain integer.

###### Totally unimodular matrix

↑ **Parent:** [Integrality of the transportation problem](#integrality-of-the-transportation-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Totally_unimodular_matrix)

A matrix is totally unimodular when every square subdeterminant is $0$, $1$, or $-1$; linear programs with such a constraint matrix and integer right side have integral vertices.

### Simplex method

↑ **Parent:** [Linear programming](#linear-programming)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplex_method)

The simplex method moves between adjacent [basic feasible solutions](#basic-feasible-solution) along improving edges of a feasible polytope until no improving pivot remains.

#### Simplex optimality criterion

↑ **Parent:** [Simplex method](#simplex-method)

In a feasible minimization [simplex dictionary](numerical-analysis.md#simplex-dictionary), the nonbasic variables are nonnegative. If every [reduced cost](#reduced-cost) $\bar c_j\ge0$, the displayed objective identity proves $z\ge z_0$ for every feasible point. Thus the current [basic feasible solution](#basic-feasible-solution) is globally optimal. If all [reduced costs](#reduced-cost) are strictly positive, equality forces every nonbasic variable to vanish and gives a unique basic solution, provided the dictionary determines all basic variables.

#### Greatest improvement pivot rule

↑ **Parent:** [Simplex method](#simplex-method)

For a feasible [simplex dictionary](numerical-analysis.md#simplex-dictionary), let $r_j>0$ be a nonbasic variable's improving [reduced cost](#reduced-cost) and let $\theta_j$ be its largest feasible increase from the [simplex ratio test](#simplex-ratio-test). The [greatest improvement pivot rule](#greatest-improvement-pivot-rule) chooses an entering variable maximizing $r_j\theta_j$. It measures the improvement over the entire edge, whereas the [Dantzig pivot rule](#dantzig-pivot-rule) maximizes only $r_j$.

// Target: mathematical-optimization.bigb

#### Dantzig pivot rule

↑ **Parent:** [Simplex method](#simplex-method)

In maximization, select the entering nonbasic variable with greatest positive [reduced cost](#reduced-cost), meaning objective increase per unit of that variable. Unlike geometric steepest-edge pricing, this rate depends on variable and constraint scaling. A rescaled [Klee-Minty cube](#klee-minty-cube) can give the same $2^n-1$-pivot path as smallest-index improving-facet pivoting.

#### Klee-Minty cube

↑ **Parent:** [Simplex method](#simplex-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klee–Minty_cube)

For $0<\varepsilon<1/2$, these inequalities define a deformed [cube](geometry-and-topology.md#cube) with $2^n$ [vertices of a polytope](#vertex-of-a-polytope). Choose either the lower or upper bound recursively at each coordinate to obtain a [vertex of a polytope](#vertex-of-a-polytope); changing one choice gives an adjacent [vertex of a polytope](#vertex-of-a-polytope). When maximizing $x_n$, smallest-index improving-facet pivoting visits all $2^n$ [vertices of a polytope](#vertex-of-a-polytope): first traverse the lower last-coordinate face, then move to the upper face and traverse the preceding path in reverse. Thus this geometric version of the [Bland pivoting rule](#bland-pivoting-rule) can require $2^n-1$ pivots. Rescaling the coordinate $x_i$ to $y_i=\varepsilon^{2(n-i)}x_i$ makes the positive rate per unit freed coordinate equal to $\varepsilon^{-(n-i)}$; [Dantzig pivot rule](#dantzig-pivot-rule) then selects the same exponential path. Euclidean edge-length pricing is a different rule.

#### Simplex tableau

↑ **Parent:** [Simplex method](#simplex-method)

A simplex tableau records the canonical constraint equations for a [simplex basis](#simplex-basis) and the canonical objective equation. For maximization use $z+\sum_j\rho_jx_j=z_0$, so a negative nonbasic objective-row coefficient is an improving direction. Constraint rows have an identity matrix in the basic columns. A [simplex method](#simplex-method) pivot divides the leaving row by the pivot coefficient and eliminates the entering column from the other rows, including the objective row. The [simplex ratio test](#simplex-ratio-test) chooses the largest feasible step. When all basic values and all $\rho_j$ are nonnegative, the objective equation directly proves $z\leq z_0$ for every nonnegative feasible vector.

##### Reconstructing a linear program from a final simplex tableau

↑ **Parent:** [Simplex tableau](#simplex-tableau)

For a maximization problem with unpriced unit [slack variables](#slack-variable), their columns in a final [simplex tableau](#simplex-tableau) give $B^{-1}$, where $B$ consists of the original basic columns. The constraint right side is $\bar b=B^{-1}b$, so $b=B\bar b$. If the objective row uses [reduced costs](#reduced-cost) $r_j=c_j-c_B^TB^{-1}A_j$, its slack entries are $-y^T$ with $y^T=c_B^TB^{-1}$. Therefore $c_B^T=y^TB$. In a homogeneous linear objective with no constant offset, the displayed basic objective value must equal $c_B^T\bar b=y^Tb$. This identity detects inconsistent tableau constants; an affine offset affects the value but not the reduced costs.

##### Simplex objective update for a priced slack variable

↑ **Parent:** [Simplex tableau](#simplex-tableau)

If a variable $x_k$ gains an objective coefficient $p$, the new objective is $z=z_{\rm old}+px_k$. Substitute this in the old canonical objective equation and eliminate any remaining basic-column coefficients using the constraint rows. If $x_k$ is nonbasic, this simply subtracts $p$ from its objective-row coefficient. When a [slack variable](#slack-variable) is sold, rename the old slack as the sales quantity; its equation already gives the correct equality and no new slack is added. Reoptimization can then start directly from the altered [simplex tableau](#simplex-tableau).

#### Bland pivoting rule

↑ **Parent:** [Simplex method](#simplex-method)

For a maximization [simplex dictionary](numerical-analysis.md#simplex-dictionary), choose the smallest-index nonbasic variable with positive reduced cost to enter. Among basic variables attaining the minimum feasible ratio, choose the smallest-index one to leave. This fixed index rule prevents cycling, including in degenerate pivots whose step length is zero. It need not minimize the number of pivots on a particular instance.

#### Two-phase simplex

↑ **Parent:** [Simplex method](#simplex-method)

Phase I introduces nonnegative artificial variables to create a feasible basis and minimizes their sum, or maximizes its negative. A positive minimum proves infeasibility. At a zero minimum, remove artificial variables and use the resulting feasible original basis in Phase II with the original objective. If an artificial variable remains basic at zero, pivot it out when possible; otherwise its row is redundant. Each phase uses the [simplex ratio test](#simplex-ratio-test) to preserve nonnegative basic values.

#### Simplex ratio test

↑ **Parent:** [Simplex method](#simplex-method)

In a feasible [simplex basis](#simplex-basis), increasing a nonbasic variable by $\theta$ changes basic coordinates to $x-\theta d$. Nonnegativity limits $\theta$ by the smallest ratio $x_i/d_i$ with $d_i>0$; a minimizing coordinate leaves the basis. Ties can leave zero-valued basic variables. This pivot test is distinct from the analytic [ratio test](real-analysis.md#ratio-test) for series convergence.

#### Simplex basis

↑ **Parent:** [Simplex method](#simplex-method)

For standard-form [linear programming](#linear-programming) constraints $Ax=b$ of full row rank, a simplex basis is a set of columns forming an invertible square matrix $B$. The remaining variables are nonbasic; setting them to zero gives the basic solution $x_B=B^{-1}b$. It is feasible if these basic variables are nonnegative. A pivot exchanges one basic and one nonbasic column while maintaining this representation.

##### Nonbasic variable

↑ **Parent:** [Simplex basis](#simplex-basis)

A [nonbasic variable](#nonbasic-variable) corresponds to a column outside the current [simplex basis](#simplex-basis). In standard nonnegative [linear programming](#linear-programming), it is set to zero at the basic solution. With explicit finite bounds, it is normally fixed at one of its bounds.

// Target: mathematical-optimization.bigb

##### Basic variable

↑ **Parent:** [Simplex basis](#simplex-basis)

A [basic variable](#basic-variable) corresponds to a column of the current [simplex basis](#simplex-basis). Given the nonbasic variables, the invertible basis matrix determines the basic variables from the equality constraints.

// Target: mathematical-optimization.bigb

##### Linear programming sensitivity within a fixed optimal basis

↑ **Parent:** [Simplex basis](#simplex-basis)

For a [linear program](#linear-programming) with unchanged cost and constraint matrix, an optimal [simplex basis](#simplex-basis) remains optimal while its basic solution remains feasible. Its [reduced costs](#reduced-cost) and dual certificate do not change. The new basic variables are $A_B^{-1}(b+\epsilon)$, and the objective is the displayed affine function, with $y$ the basis's dual solution. This gives an exact piecewise-affine sensitivity region, determined by nonnegativity of the basic variables, rather than merely a formal first derivative.

###### Strictly positive dual certificate and right-hand-side sensitivity

↑ **Parent:** [Linear programming sensitivity within a fixed optimal basis](#linear-programming-sensitivity-within-a-fixed-optimal-basis)

For a square invertible constraint matrix $A$ in $\max\{c^Tx:Ax\leq b,x\geq0\}$, suppose $y>0$ and $A^Ty=c$. This fixed dual vector stays optimal under a changed right-hand side $b'$ exactly when $A^{-1}b'\geq0$. Sufficiency follows from primal feasibility and equal primal/dual objectives. Necessity follows from [complementary slackness](#complementary-slackness): since every $y_i$ is positive, every optimal primal constraint must bind, forcing $x=A^{-1}b'$. The inequalities define the whole validity cone, including degenerate boundary optima.

#### Simplex paths on a cube with one truncated corner

↑ **Parent:** [Simplex method](#simplex-method)

For $0\leq x_i\leq1$, $x_1+x_2+x_3\leq5/2$, and objective $x_1+2x_2+4x_3$, the oriented edge graph has eight improving paths from the origin to the unique optimum $(1/2,1,1)$. Their lengths range from three to five pivots.

## Convex set

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_set)

A convex set contains every [line segment](#line-segment) joining two of its points.

### Hyperplane separation theorem

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperplane_separation_theorem)

Two nonempty disjoint [convex sets](#convex-set) in a finite-dimensional real [vector space](vector-space.md) admit a separating nonzero [linear functional](linear-algebra.md#linear-functional): for an appropriate $h\ne0$ and $a$, $h\cdot x\leq a\leq h\cdot y$ on the respective sets. Strict separation requires additional assumptions, such as one set being compact and the other closed. For an open [convex cone](#convex-cone) $C$ excluding zero, separation from $\{0\}$ gives $h\cdot c\geq0$ for all $c\in C$; scaling cone elements forces the separating level to be zero. This finite-dimensional result is related to the [supporting hyperplane theorem](#supporting-hyperplane-theorem).

### Supporting hyperplane theorem

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supporting_hyperplane_theorem)

A [convex set](#convex-set) in a finite-dimensional space has a nonzero supporting linear functional at each boundary point. If zero lies outside a nonempty [convex set](#convex-set) $C$, weak separation gives $p\ne0$ with $p\cdot c\geq0$ for all $c\in C$, even when zero belongs to its closure. Strict separation needs stronger hypotheses.

### Relative interior

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Relative_interior)

The relative interior of a convex set is its interior in its affine span. A polyhedral cone has nonempty relative interior in its linear span, even when its ordinary interior in the ambient vector space is empty.

// Target: geometry-and-topology.bigb

### Radially open convex set

↑ **Parent:** [Convex set](#convex-set)

A subset $C$ of a real [vector space](vector-space.md) is radially open when, for each $x\in C$ and each vector $v$, the points $x+tv$ remain in $C$ for all sufficiently small real $t$. No ambient topology is required. If $C$ is also convex and contains zero, it is absorbing and its [Minkowski functional](topological-vector-space.md#minkowski-functional) $p_C(x)=\inf\{s>0:x\in sC\}$ is finite and sublinear, with $C=\{p_C<1\}$. Convexity gives subadditivity; radial openness permits a slight dilation of any point of $C$, giving the strict inequality.

### Half-space representation of a closed convex set

↑ **Parent:** [Convex set](#convex-set)

A closed [convex set](#convex-set) in a finite-dimensional Euclidean space is the intersection of all containing [closed half-spaces](#closed-half-space). For a point outside a nonempty set, its [Euclidean projection onto a convex set](#euclidean-projection-onto-a-convex-set) gives a separating normal. Applied to an [epigraph](calculus-of-variations.md#epigraph), this turns geometric separation into affine lower bounds and is a key step in the [Fenchel-Moreau theorem](convex-optimization.md#fenchel-moreau-theorem).

### Recession cone

↑ **Parent:** [Convex set](#convex-set)

The recession cone of a nonempty [convex set](#convex-set) $C$ consists of directions $d$ for which $x+td\in C$ for every $x\in C$ and $t\ge0$. For a [linear polyhedron](#linear-polyhedron) $P=\{x:Ax\le b\}$ it is exactly $\{d:Ad\le0\}$. A nonzero recession direction gives an unbounded ray, so a bounded nonempty polyhedron has recession cone $\{0\}$. This excludes spurious zero-scale feasible points in the [Charnes-Cooper transformation](#charnes-cooper-transformation).

### Face of a convex set

↑ **Parent:** [Convex set](#convex-set)

A [convex set](#convex-set) $F\subseteq C$ is a face of $C$ if $ty+(1-t)z\in F$, with $y,z\in C$ and $0<t<1$, implies $y,z\in F$. A singleton face is an [extreme point](#extreme-point). A face of a face is a face of the original [convex set](#convex-set).

### Compact convex set

↑ **Parent:** [Convex set](#convex-set)

A [compact convex set](#compact-convex-set) $K\subseteq\mathbb R^n$ is a [compact set](topology.md#compact-space) that is also a [convex set](#convex-set). If $K$ is nonempty, its [support function](#support-function) $H_K(\eta)=\max_{x\in K}x\cdot\eta$ is finite in every direction. For such a nonempty $K$, every exterior point $x_0$ admits a strictly [separating hyperplane](statistical-learning.md#separating-hyperplane): minimize $|x_0-y|$ over $y\in K$, and put $\omega=x_0-y$. Convexity and differentiation along the segment from $y$ to any $z\in K$ give $\omega\cdot(z-y)\leq0$, while $\omega\cdot(x_0-y)=|\omega|^2>0$. This is the separation used to recover spatial support from Fourier growth.

### Nonnegative orthant

↑ **Parent:** [Convex set](#convex-set)

The nonnegative orthant consists of vectors whose coordinates are all nonnegative. Its interior is the positive orthant, where every coordinate is positive.

It is the closed [orthant](#orthant) obtained by choosing the nonnegative sign for every coordinate.

### Convex combination

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_combination)

A convex combination of points $x_1,\ldots,x_n$ is a sum

$$
\sum_{i=1}^n\lambda_i x_i,
\qquad \lambda_i\geq0,
\qquad \sum_{i=1}^n\lambda_i=1.
$$

#### Cyclic symmetry averaging

↑ **Parent:** [Convex combination](#convex-combination)

If a convex subset of $\mathbb R^n$ is invariant under cyclic coordinate permutation, averaging the $n$ cyclic images of $x$ shows that

$$
\left(\frac1n\sum_jx_j,\ldots,\frac1n\sum_jx_j\right)
$$

also belongs to the set.

### Closed half-space

↑ **Parent:** [Convex set](#convex-set)

A closed half-space is a set of the form $\{x:a^Tx\leq b\}$ for a nonzero vector $a$; it is a [convex set](#convex-set) and is closed.

This is the non-strict version of a [half-space](geometry-and-topology.md#half-space); replacing the inequality by a strict one gives the open version.

### Line segment

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Line_segment)

The line segment joining vectors $x$ and $y$ is

$$
\{(1-t)x+ty:0\leq t\leq1\}.
$$

#### Midpoint

↑ **Parent:** [Line segment](#line-segment)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Midpoint)

The midpoint of the [line segment](#line-segment) joining two points with position vectors $a,b$ is the point $m=(a+b)/2$. Its displacements from the endpoints are $(b-a)/2$ and $(a-b)/2$, so it lies on the segment and is equidistant from its endpoints. It is also the [centroid](geometry-and-topology.md#centroid) of the two endpoints.

#### Closest points on two line segments

↑ **Parent:** [Line segment](#line-segment)

For [line segments](#line-segment) $P+sd$ and $Q+te$, $0\leq s,t\leq1$, the squared [Euclidean distance](topological-analysis.md#euclidean-distance) is a [convex quadratic function](real-analysis.md#convex-quadratic-function) on a square. Its minimum is either an admissible stationary point or a minimum on one of the four edges. Each edge minimum is a point-to-segment [orthogonal projection](hilbert-space.md#orthogonal-projection), restricted to the interval. Testing these five candidates gives a complete algorithm; when the directions are parallel, the edge candidates suffice. Independently restricting both coordinates of the unconstrained stationary point is generally incorrect because the variables are coupled by $d\cdot e$.

##### Contact time of translating line segments

↑ **Parent:** [Closest points on two line segments](#closest-points-on-two-line-segments)

For segments with initial direction vectors $U,T$, initial endpoint displacement $D$, and translation velocities $V,W$, contact is feasibility of the displayed [linear equation](linear-algebra.md#linear-equation) with $s,r\in[0,1]$ and $t\ge0$. Minimizing $t$ is a small [linear programming](#linear-programming) problem. A nonsingular three-column coefficient [matrix](vector-space.md#matrix) gives at most one candidate; singular, parallel and degenerate cases require the constrained feasibility problem rather than division by a vanishing [determinant](linear-algebra.md#determinant).

###### Proximity time of translating line segments

↑ **Parent:** [Contact time of translating line segments](#contact-time-of-translating-line-segments)

The earliest approach within distance $d$ is a [convex optimization](convex-optimization.md) problem with a norm constraint and the same segment and time bounds as contact. An elementary alternative enumerates whether each segment parameter is free or at an endpoint. In each nonsingular active case the free closest-point parameters are [affine functions](vector-space.md#affine-function) of time, leaving a quadratic distance inequality on a valid time interval. Rank-deficient cases need their null-space constraints retained. Unlike contact, the two segment parameters and time are no longer determined by a vector equality.

### Convex polytope

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_polytope)

A convex polytope is a bounded intersection of finitely many closed half-spaces, equivalently the convex hull of finitely many points.

#### Zonotope

↑ **Parent:** [Convex polytope](#convex-polytope)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zonotope)

A [zonotope](#zonotope) is a [Minkowski sum](geometry-and-topology.md#minkowski-addition) of finitely many [line segments](#line-segment), equivalently an [affine map](geometry-and-topology.md#affine-map) image of a cube. For vectors $\xi_j$, the set $\sum_j[0,1]\xi_j$ is the support of the associated [box spline](uniform-approximation.md#box-spline). A centred version uses $[-1/2,1/2]\xi_j$ instead. In two dimensions, sums of differently directed segments give centrally symmetric polygons; repeated directions lengthen their corresponding edges without adding new edge directions.

#### Lattice polytope

↑ **Parent:** [Convex polytope](#convex-polytope)

A lattice polytope is the convex hull of finitely many points of a [Euclidean lattice](fourier-analysis.md#euclidean-lattice). It need not contain the origin. Integral translation changes its associated homogeneous semigroup ring by a grading-preserving isomorphism.

// Target: geometry-and-topology.bigb

#### Convex polygon

↑ **Parent:** [Convex polytope](#convex-polytope)

A convex polygon is a two-dimensional [convex polytope](#convex-polytope), equivalently the [convex hull](#convex-hull) of a finite planar set with nonempty interior. Its vertices are the extreme points of that hull. Saying that given points form a convex polygon means every specified point is a vertex; points inside the hull or in the interior of a straight boundary segment do not count as vertices.

##### Convex chain

↑ **Parent:** [Convex polygon](#convex-polygon)

A convex chain between two fixed points inside a [triangle](geometry-and-topology.md#triangle) is a finite point set whose union with the endpoints forms the vertices of a [convex polygon](#convex-polygon), with the endpoint segment as one boundary edge. In the triangle $0\leq y\leq x\leq1$, with endpoints $(0,0)$ and $(1,1)$, its ordered lower boundary has strictly increasing segment slopes. Every subset of its intermediate vertices remains a convex chain. This hereditary property lets selected point coordinates certify the existence of a long chain.

###### Convex-chain probability in a triangle

↑ **Parent:** [Convex chain](#convex-chain)

For independent uniform points in $0\leq y\leq x\leq1$ with the two diagonal endpoints, the displayed formula is exact. Order the $k$ intermediate points so that both coordinates increase, and write the $k+1$ positive coordinate spacings as $(u_i)$ and $(v_i)$, with each sum equal to one. The two spacing vectors have uniform simplex measure, independently, and the full ordered-coordinate region has volume $1/(k!)^2$. Simultaneous permutation of the spacing pairs preserves that measure, so all $(k+1)!$ orders of the ratios $v_i/u_i$ have equal volume. Strictly increasing ratios characterize a convex chain and automatically place the intermediate points below the diagonal. Thus its ordered volume is $1/((k!)^2(k+1)!)$. There are $k!$ ways to assign labels, and uniform triangle density is $2^k$, giving the formula. Consequently the [first moment method](probability-inequality.md#first-moment-method) bounds the probability of any length-$k$ chain among $n$ points by $\binom nk2^k/(k!(k+1)!)$.

###### Longest convex chain

↑ **Parent:** [Convex chain](#convex-chain)

For $n$ points in a [triangle](geometry-and-topology.md#triangle) and two fixed endpoint vertices, the longest convex chain length is the largest number of sampled points in a [convex chain](#convex-chain) joining those endpoints. It is a [certifiable function](probability-inequality.md#certifiable-function): a chain of length $a$ supplies a certificate of exactly $a$ point coordinates. Changing one point changes the maximum by at most one, since deleting that point from any optimal chain loses at most one vertex. For independent uniform points, its [median](probability-theory.md#median) is $O(n^{1/3})$ and its fluctuation scale about the median is at most $n^{1/6}$, as proved by [convex-chain probability in a triangle](#convex-chain-probability-in-a-triangle) and [convex-chain median concentration](#convex-chain-median-concentration).

###### Convex-chain median concentration

↑ **Parent:** [Longest convex chain](#longest-convex-chain)

Let $m$ be an integer [median](probability-theory.md#median) for the [longest convex chain](#longest-convex-chain) length of independent uniform points in a [triangle](geometry-and-topology.md#triangle). If $L_n(x)\geq a$, fix a certificate of $a$ coordinates. Every configuration with $L_n\leq b$ must disagree with at least $a-b$ of those coordinates; equal weights $1/\sqrt a$ prove [Talagrand convex distance](probability-inequality.md#talagrand-convex-distance) separation at least $(a-b)/\sqrt a$. [Talagrand's convex distance inequality](probability-inequality.md#talagrand-s-convex-distance-inequality) then gives $\mathbb P(L_n\geq a)\mathbb P(L_n\leq b)\leq e^{-(a-b)^2/(4a)}$. Set $b=m$, then $a=m$, in the two respective applications to obtain the displayed tails for positive integer $t$. The exact chain-counting bound gives $m\leq Cn^{1/3}$. Hence any interval centred at $m$ with length $\omega(n)n^{1/6}$, where $\omega(n)\to\infty$, contains $L_n$ [with high probability](probabilistic-combinatorics.md#with-high-probability). No upper restriction on the growth of $\omega$ is required.

#### Vertex of a polytope

↑ **Parent:** [Convex polytope](#convex-polytope)

A vertex of a [convex polytope](#convex-polytope) is an [extreme point](#extreme-point): it cannot be expressed as a nontrivial convex combination of two distinct points in that polytope. In a full-dimensional simple polytope of dimension $n$, a vertex lies on exactly $n$ incident [facets](#facet).

#### Facet

↑ **Parent:** [Convex polytope](#convex-polytope)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Facet_(geometry))

A facet of a full-dimensional [convex polytope](#convex-polytope) in $\mathbb R^n$ is a face of dimension $n-1$. Each irredundant supporting [closed half-space](#closed-half-space) defines one facet.

##### Facet lower bound for ball approximations

↑ **Parent:** [Facet](#facet)

If $r\geq\sqrt2$ and a [convex polytope](#convex-polytope) satisfies $r^{-1}B^n\subseteq P\subseteq B^n$, then it has at least $(1-r^{-2})^{-n/2}\geq e^{n/(2r^2)}$ [facets](#facet). Its outward facet normals define [spherical caps](geometry-and-topology.md#spherical-cap) covering the [unit sphere](topology.md#unit-sphere); the [spherical cap area upper bound](geometry-and-topology.md#spherical-cap-area-upper-bound) supplies the estimate.

#### Cross-polytope

↑ **Parent:** [Convex polytope](#convex-polytope)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-polytope)

The [convex hull](#convex-hull) of the positive and negative coordinate [unit vectors](vector-space.md#unit-vector). Its boundary triangulates a [sphere](geometry-and-topology.md#sphere), and each face contains at most one member of each antipodal pair of coordinate [unit vectors](vector-space.md#unit-vector). This makes its [barycentric subdivision](homology.md#barycentric-subdivision) useful for triangulating [Real projective space](algebraic-topology.md#real-projective-space).

### Extreme point

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extreme_point)

An extreme point of a convex set $C$ is a point $x\in C$ for which

$$
x=(1-t)y+tz,\qquad y,z\in C,\quad0<t<1
$$

implies $x=y=z$.

#### Extreme points of real sequence-space unit balls

↑ **Parent:** [Extreme point](#extreme-point)

For the real [l-infinity sequence space](banach-space.md#l-infinity-sequence-space), every coordinate of an [extreme point](#extreme-point) must be an endpoint of $[-1,1]$; any slack coordinate permits opposite perturbations. For the real [absolutely summable sequence space](banach-space.md#absolutely-summable-sequence-space), a unit vector with two nonzero coordinates permits a transfer of mass between them, so only signed coordinate vectors are extreme. For the real [l2 sequence space](banach-space.md#l2-sequence-space), the [parallelogram law](linear-algebra.md#parallelogram-law) makes every unit vector extreme. In all three cases interior points of the unit ball are nonextreme.

#### Extreme points of a real continuous-function unit ball

↑ **Parent:** [Extreme point](#extreme-point)

For compact Hausdorff $K$, the extreme points of the real unit ball in the [space of continuous functions on a compact space](functional-analysis.md#space-of-continuous-functions-on-a-compact-space) are precisely its continuous sign-valued functions. A point with $|f|<1$ permits a nonzero continuous bump perturbation supported where there is uniform slack, while pointwise equality at an endpoint of $[-1,1]$ forces both functions in a midpoint decomposition to agree. For the [Cantor set](geometry-and-topology.md#cantor-set), [clopen](topology.md#clopen-set) indicators give the perturbations directly.

##### Clopen sign approximation in the real Cantor unit ball

↑ **Parent:** [Extreme points of a real continuous-function unit ball](#extreme-points-of-a-real-continuous-function-unit-ball)

Every real continuous function of supremum norm at most one on the [Cantor set](geometry-and-topology.md#cantor-set) is a uniform limit of convex combinations of continuous sign functions. Approximate on a finite [Cantor cylinder](geometry-and-topology.md#cantor-cylinder) partition by values $a_j\in[-1,1]$. The sign vector $s$ has weight $\prod_j(1+s_ja_j)/2$, whose coordinate means are $a_j$. This proves a [closed convex hull](#closed-convex-hull) identity without weak compactness.

#### Extreme-point criterion for the L-infinity unit ball

↑ **Parent:** [Extreme point](#extreme-point)

For real scalars the extremes are the almost-everywhere sign-valued [functions](function.md). A positive-[measure](measure-theory.md#measure) region uniformly inside $[-1,1]$ permits opposite nontrivial bounded perturbations, proving necessity. Equality at either endpoint forces both members of a convex decomposition to agree, proving sufficiency. For complex scalars the same criterion uses unit-modulus [functions](function.md) and the strict convexity of the complex unit disk.

### Projections onto convex sets

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projections_onto_convex_sets)

[Projections onto convex sets](#projections-onto-convex-sets) is an iterative feasibility method that successively applies a [Euclidean projection onto a convex set](#euclidean-projection-onto-a-convex-set) to each closed convex constraint set. With two sets it uses $x_{n+1}=P_D(P_C(x_n))$. It seeks a point in the intersection; a single projection onto one set is a different operation, and the method does not generally compute the closest intersection point to the initial iterate.

### Euclidean projection onto a convex set

↑ **Parent:** [Convex set](#convex-set)

For a nonempty closed convex subset $C$ of a finite-dimensional inner-product space, $\Pi_C(x)$ is the unique point of $C$ minimizing $\|x-z\|$.

This closest-point map is the [metric projection onto a closed convex set](#euclidean-projection-onto-a-convex-set). Repeated projections onto several sets form the separate [projections onto convex sets](#projections-onto-convex-sets) method.

#### Variational characterization of convex projection

↑ **Parent:** [Euclidean projection onto a convex set](#euclidean-projection-onto-a-convex-set)

For $p\in C$,

$$
p=\Pi_C(x)
\quad\Longleftrightarrow\quad
\langle x-p,z-p\rangle\leq0
\quad\text{for every }z\in C.
$$

#### Nonexpansiveness of metric projection

↑ **Parent:** [Euclidean projection onto a convex set](#euclidean-projection-onto-a-convex-set)

The metric projection onto a nonempty closed convex set in a Hilbert space is nonexpansive:

$$
\lVert\Pi_C(x)-\Pi_C(y)\rVert\leq\lVert x-y\rVert.
$$

#### Projection onto a box-constrained hyperplane

↑ **Parent:** [Euclidean projection onto a convex set](#euclidean-projection-onto-a-convex-set)

For $C=\{x:0\leq x\leq1,\ a^Tx=b\}$, the projection of $y$ has coordinates $x_i=\min(1,\max(0,y_i-\nu a_i))$, where the scalar multiplier $\nu$ is chosen so that $a^Tx=b$. Thus the projection reduces to a continuous one-dimensional root-finding problem.

### Support function

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Support_function)

The support function of a nonempty set $C$ is $\sigma_C(x)=\sup_{v\in C}\langle x,v\rangle$. It is convex and positively homogeneous, and for a closed convex set its [convex conjugate](convex-optimization.md#convex-conjugate) is the [indicator function](measure-theory.md#indicator-function) of $C$.

#### Support-function subgradients as exposed faces

↑ **Parent:** [Support function](#support-function)

For a nonempty closed [convex set](#convex-set) $C$, the finite-valued [support function](#support-function) has [subgradients](real-analysis.md#subgradient) exactly at the maximizing points of $C$. This follows from [Fenchel–Young inequality](convex-optimization.md#fenchel-young-inequality) and the conjugacy between the [support function](#support-function) and the [indicator functional of a constraint set](inverse-problem.md#indicator-functional-of-a-constraint-set). For compact $C$, the exposed maximizing set is nonempty.

#### Support function of an inverse image of an infinity-norm ball

↑ **Parent:** [Support function](#support-function)

If $x\notin\operatorname{range}P^T=(\ker P)^\perp$, the [support function](#support-function) is infinite along a kernel line. Otherwise [linear programming duality](#linear-programming-duality) gives the displayed minimum, attained because the corresponding linear programs are feasible with finite values. Splitting $q=\alpha-\beta$ into nonnegative parts yields the equivalent minimum of $\mathbf1^T(\alpha+\beta)$. Thus worst-case revenue over a [polyhedral uncertainty set](convex-optimization.md#polyhedral-uncertainty-set) is $r_0^Tx-\sigma_C(x)$, with value $-\infty$ off the row space.

#### Sum of the largest components

↑ **Parent:** [Support function](#support-function)

The sum of the $k$ largest components of $x\in\mathbb R^n$ is the [support function](#support-function) of the [capped simplex](#capped-simplex): $\sum_{i=1}^k x_{[i]}=\max\{x^Tv:0\leq v\leq1,\ \sum_i v_i=k\}$.

##### Threshold formula for the sum of the largest components

↑ **Parent:** [Sum of the largest components](#sum-of-the-largest-components)

For $1\leq k\leq n$, [linear programming duality](#linear-programming-duality) gives

$$
f_k(x)=\min_{t\in\mathbb R,\ s\geq0}\left\{kt+\sum_i s_i:s_i+t\geq x_i\right\}
=\min_{t\in\mathbb R}\left\{kt+\sum_i(x_i-t)_+\right\},
$$

where $(\cdot)_+$ is the [positive part of a real-valued function](function.md#positive-part-of-a-real-valued-function). To see equality directly, order the coordinates $x_{[1]}\geq\cdots\geq x_{[n]}$ and choose $x_{[k+1]}\leq t\leq x_{[k]}$ for $k<n$, or $t\leq x_{[n]}$ for $k=n$. The threshold expression then equals the [sum of the largest components](#sum-of-the-largest-components). Introducing the variables $s_i$ turns this [convex](real-analysis.md#convex-function) piecewise-linear objective into a [linear program](#linear-programming).

#### Sum of the largest eigenvalues

↑ **Parent:** [Support function](#support-function)

For a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $X$ with [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_1\geq\cdots\geq\lambda_n$, the sum of its $k$ largest [eigenvalues](linear-operator-theory.md#eigenvalue) is the [support function](#support-function) of the [fantope](#fantope):

$$
F_k(X)=\max\{\operatorname{tr}(XY):0\preceq Y\preceq I,\ \operatorname{tr}Y=k\}.
$$

Here $\preceq$ is the [Loewner order](linear-algebra.md#loewner-order). In an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) for $X$, the objective depends only on the diagonal entries of $Y$, which lie in the [capped simplex](#capped-simplex). Thus the identity reduces to the [sum of the largest components](#sum-of-the-largest-components) of the [eigenvalues](linear-operator-theory.md#eigenvalue).

##### Ky Fan maximum principle

↑ **Parent:** [Sum of the largest eigenvalues](#sum-of-the-largest-eigenvalues)

For a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $X$ and $1\leq k\leq n$,

$$
\sum_{i=1}^k\lambda_i(X)
=\max_{Q^TQ=I_k}\operatorname{tr}(Q^TXQ).
$$

Indeed $Y=QQ^T$ is a rank-$k$ [orthogonal projection matrix](linear-algebra.md#orthogonal-projection-matrix) in the [fantope](#fantope), and projecting onto the [eigenvectors](linear-operator-theory.md#eigenvector) of the largest [eigenvalues](linear-operator-theory.md#eigenvalue) attains the [support function](#support-function) maximum. Equivalently, the largest [matrix trace](linear-algebra.md#matrix-trace) of a compression to a $k$-dimensional [vector subspace](vector-space.md#vector-subspace) is the [sum of the largest eigenvalues](#sum-of-the-largest-eigenvalues).

###### Hermitian effect variational principle

↑ **Parent:** [Ky Fan maximum principle](#ky-fan-maximum-principle)

For a finite-dimensional [Hermitian operator](hilbert-space.md#hermitian-operator) $A$ with decreasing [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_j$ and integer $0\leq r\leq d$, maximizing $\operatorname{Tr}(AB)$ over [positive contractions](hilbert-space.md#positive-contraction) $B$ with [trace](linear-algebra.md#matrix-trace) $r$ gives the sum of its leading $r$ [eigenvalues](linear-operator-theory.md#eigenvalue). In an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis), the diagonal entries of $B$ lie in $[0,1]$ and sum to $r$. Moving their weight to the largest [eigenvalues](linear-operator-theory.md#eigenvalue) can only increase the objective. An [orthogonal projection](hilbert-space.md#orthogonal-projection) onto their [eigenvectors](linear-operator-theory.md#eigenvector) attains the maximum.

##### Threshold semidefinite program for the largest eigenvalues

↑ **Parent:** [Sum of the largest eigenvalues](#sum-of-the-largest-eigenvalues)

The [sum of the largest eigenvalues](#sum-of-the-largest-eigenvalues) has the [semidefinite program](convex-optimization.md#semidefinite-programming) representation

$$
F_k(X)=\min_{t\in\mathbb R,\ S\succeq0}\{kt+\operatorname{tr}S:S\succeq X-tI\}.
$$

For every feasible $Y$ in the [fantope](#fantope), [positive semidefinite trace nonnegativity](linear-algebra.md#positive-semidefinite-trace-nonnegativity) gives $\operatorname{tr}(XY)\leq kt+\operatorname{tr}S$. To attain equality, use an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) of $X$ and choose $S=\operatorname{diag}((\lambda_i-t)_+)$ in that basis, with the same threshold choice as in the [threshold formula for the sum of the largest components](#threshold-formula-for-the-sum-of-the-largest-components). This argument also covers $k=n$, without requiring strict feasibility of the maximization program.

### Capped simplex

↑ **Parent:** [Convex set](#convex-set)

For an integer $0\leq k\leq n$, the capped simplex

$$
P_k=\{v\in\mathbb R^n:0\leq v_i\leq1,\ \sum_i v_i=k\}
$$

is the [convex hull](#convex-hull) of the zero-one [vectors](vector-space.md#vector) having exactly $k$ entries equal to one. It is a [convex polytope](#convex-polytope) whose [extreme points](#extreme-point) are precisely these [vectors](vector-space.md#vector).

If a feasible [vector](vector-space.md#vector) has a fractional coordinate, the integer coordinate sum forces at least two fractional coordinates. Perturbing one upward and the other downward by a sufficiently small amount gives two distinct feasible [vectors](vector-space.md#vector) whose midpoint is the original [vector](vector-space.md#vector). It is therefore not an [extreme point](#extreme-point). Conversely, a zero-one [vector](vector-space.md#vector) cannot be a nontrivial [convex combination](#convex-combination) of points of $[0,1]^n$, since each coordinate is already at a bound.

### Second-order cone

↑ **Parent:** [Convex set](#convex-set)

The second-order cone, also called the Lorentz cone, is

$$
\mathcal L_{p+1}=\{(v,s)\in\mathbb R^p\times\mathbb R:\|v\|_2\leq s\}.
$$

#### Self-duality of a second-order cone

↑ **Parent:** [Second-order cone](#second-order-cone)

For $(u,s),(v,t)$ in the [second-order cone](#second-order-cone), the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $u\cdot v+st\ge-\|u\|\|v\|+st\ge0$. Thus the cone is contained in its [dual cone](toric-geometry.md#dual-cone). Conversely, if $s<\|u\|$ and $u\ne0$, pairing $(u,s)$ with $(-u/\|u\|,1)$ is negative. If $u=0$ and $s<0$, use $(0,1)$. Every point outside the cone therefore lies outside its dual, proving that it is a [self-dual cone](#self-dual-cone).

#### Second-order cone programming

↑ **Parent:** [Second-order cone](#second-order-cone)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second-order_cone_programming)

A second-order cone program has a linear objective and affine constraints taking values in products of [second-order cones](#second-order-cone) and nonnegative orthants. Norm epigraphs have the form $(t,z)\in\mathcal Q$; quadratic epigraphs admit the affine lift $((q+1)/2,(q-1)/2,a)\in\mathcal Q_3$, equivalent to $q\geq a^2$. Product-cone [self-concordant barriers](convex-optimization.md#self-concordant-barrier) give [interior-point methods](convex-optimization.md#interior-point-method).

##### Second-order cone reformulation of one-sided quadratic denoising

↑ **Parent:** [Second-order cone programming](#second-order-cone-programming)

The objective $\|u-g\|_2+\lambda\sum_i((Gu)_i)_+^2$ has the exact lift $\min t+\lambda\sum_iq_i$ with $(t,u-g)\in\mathcal Q_{n+1}$, $((q_i+1)/2,(q_i-1)/2,a_i)\in\mathcal Q_3$, $a_i\geq0$ and $a_i\geq(Gu)_i$. Every lifted feasible value bounds the original objective, and choosing tight epigraph variables proves equality. The product-cone barrier parameter is $4n+2$: two for each Lorentz block and one for each orthant slack. The fidelity norm remains unsquared, and negative derivatives remain unpenalized.

#### Projection onto the second-order cone

↑ **Parent:** [Second-order cone](#second-order-cone)

For $x=(u,t)$ and $\rho=\|u\|_2$,

$$
\Pi_{\mathcal L_{p+1}}(u,t)=
\begin{cases}
(u,t),&\rho\leq t,\\
(0,0),&\rho\leq-t,\\
\displaystyle\frac12\left(1+\frac t\rho\right)(u,\rho),&\rho>|t|.
\end{cases}
$$

### Convex hull

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_hull)

The convex hull of a set is the set of all finite convex combinations of its points, equivalently the smallest convex set containing it.

#### Closed convex hull

↑ **Parent:** [Convex hull](#convex-hull)

The smallest closed [convex set](#convex-set) containing a set $C$, equivalently the closure of its [convex hull](#convex-hull) in the specified [topology](topology.md). The topology must be stated: the [norm topology](functional-analysis.md#norm-topology), [weak topology](weak-topology.md) and [weak-star topology](weak-topology.md#weak-star-topology) need not give the same closure for an arbitrary set.

<h4 id="caratheodory-s-theorem-convex-hull">Carathéodory's theorem (convex hull)</h4>

↑ **Parent:** [Convex hull](#convex-hull)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carathéodory's_theorem_(convex_hull))

Every point in the convex hull of a subset of $\mathbb R^d$ is a convex combination of at most $d+1$ points of that subset.

<h5 id="conic-caratheodory-theorem">Conic Carathéodory theorem</h5>

↑ **Parent:** [Carathéodory's theorem (convex hull)](#caratheodory-s-theorem-convex-hull)

In an $N$-dimensional real [vector space](vector-space.md), each member of a [conic hull](#conic-hull) has a representation using at most $N$ generators. To prove it, take a finite positive-coefficient representation with more than $N$ terms. Its generators are linearly dependent, say $\sum_j\mu_js_j=0$, with some $\mu_j>0$ after reversing the relation if necessary. Subtract $t\mu_j$ from each [coefficient](vector-space.md#coefficient), taking $t=\min_{\mu_j>0}\lambda_j/\mu_j$. All [coefficients](vector-space.md#coefficient) stay nonnegative and at least one vanishes. Iterate. The bound differs from the $N+1$ bound for a [convex hull](#convex-hull) because the [coefficient](vector-space.md#coefficient) sum is unrestricted.

### Convex cone

↑ **Parent:** [Convex set](#convex-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_cone)

A convex cone is a subset $C$ of a real [vector space](vector-space.md) closed under nonnegative [linear combinations](vector-space.md#linear-combination): $ax+by\in C$ whenever $x,y\in C$ and $a,b\geq0$. The [positive semidefinite cone](#positive-semidefinite-cone) and the [copositive cone](#copositive-cone) are examples, ordered by inclusion through the [positive-semidefinite-plus-nonnegative cone](#positive-semidefinite-plus-nonnegative-cone).

#### Orthant

↑ **Parent:** [Convex cone](#convex-cone)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthant)

A closed coordinate-sign region of [Euclidean space](functional-analysis.md#euclidean-norm). The $2^n$ orthants cover the space. An orthant contains no nontrivial affine line: for a nonzero direction, some coordinate eventually violates its sign restriction in one direction. Adding orthant inequalities to a nonempty [linear polyhedron](#linear-polyhedron) therefore permits construction of a [basic feasible solution](#basic-feasible-solution) even when the original polyhedron has no vertex.

#### Strictly positive barycentre cone lemma

↑ **Parent:** [Convex cone](#convex-cone)

For a finite-dimensional [random vector](random-variable.md#random-vector) $X$, let $K$ be the closed cone generated by the [support of a probability distribution](probability-theory.md#support-of-a-probability-distribution) of $X$. Every integrable strictly positively weighted barycentre lies in the [relative interior](#relative-interior) of $K$: every nonzero supporting functional on its span is positive on a set of positive probability. Conversely, put $w=(1+\|X\|)^{-1}$ and $D=\{\mathbb E[w fX]:0\leq f\in L^\infty\}$. Its dual cone equals that of $K$, so $\overline D=K$ and $\operatorname{ri}K\subseteq D$. For $z\in\operatorname{ri}K$, subtract a sufficiently small positive multiple of $\mathbb E[wX]$ and represent the remainder using $D$; adding the constant positive weight back gives $\nu=w(f+\varepsilon)>0$.

##### Positive-weight expectation cone

↑ **Parent:** [Strictly positive barycentre cone lemma](#strictly-positive-barycentre-cone-lemma)

For an [integrable](measure-theory.md#integrability) finite-dimensional [random vector](random-variable.md#random-vector) $Y$, let $L=\{h:h\cdot Y=0\text{ almost surely}\}^\perp$. The displayed [convex cone](#convex-cone) is open relative to $L$. Given a bounded strictly positive $Z$, the perturbation $Z_\varepsilon=Z(1+\varepsilon\cdot Y/(1+\|Y\|))$, $\|\varepsilon\|<1$, changes its weighted [expectation](probability-theory.md#expected-value) by $A_Z\varepsilon$, where

$$
A_Z=\mathbb E\frac{ZYY^T}{1+\|Y\|}.
$$

For $0\ne v\in L$, $v^TA_Zv>0$: otherwise $v\cdot Y=0$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence). Thus $A_Z$ is invertible on $L$, and these perturbations give a neighborhood of every point of the cone. The [hyperplane separation theorem](#hyperplane-separation-theorem) consequently gives the alternative: either zero is a strictly positively weighted [expectation](probability-theory.md#expected-value), or a nonzero direction in $L$ has a nonnegative [dot product](linear-algebra.md#dot-product) with $Y$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence) and a positive [dot product](linear-algebra.md#dot-product) with positive [probability](probability-theory.md#probability). To obtain the latter assertion, test the separating direction with $Z=\mathbf1_{\{h\cdot Y<0\}}+\varepsilon$ and let $\varepsilon\downarrow0$.

#### Support-minimal rays of a nonnegative kernel

↑ **Parent:** [Convex cone](#convex-cone)

Every nonzero vector of $K$ is a nonnegative combination of at most as many support-minimal vectors as it has nonzero coordinates. Choose a nonnegative kernel vector $h$ of minimal nonempty support inside the support of $u$; subtract $\lambda h$, where $\lambda=\min_{h_i>0}u_i/h_i$. The remainder is nonnegative, remains in the kernel, and has strictly smaller support. Induction proves the decomposition. On a minimal support, the kernel is one-dimensional: an independent kernel direction could perturb a strictly positive vector to the boundary of that support without making it zero, contradicting minimality. For an integer matrix with entries bounded by $M$, cofactor determinants give an integer generator with coordinates bounded by $q!M^q$, where $q$ is the ambient number of coordinates.

#### Lineality space

↑ **Parent:** [Convex cone](#convex-cone)

The lineality space of a convex cone is its largest linear subspace, equal to $C\cap(-C)$. Every nonempty face contains it. A cone is pointed exactly when this space is zero.

// Target: mathematical-optimization.bigb

#### Self-dual cone

↑ **Parent:** [Convex cone](#convex-cone)

A [self-dual cone](#self-dual-cone) equals its [dual cone](toric-geometry.md#dual-cone) under the specified inner product. The [nonnegative orthant](#nonnegative-orthant), [second-order cone](#second-order-cone) and [positive semidefinite cone](#positive-semidefinite-cone) are standard examples. Self-duality of a set alone does not establish primal or dual feasibility.

#### Proper cone

↑ **Parent:** [Convex cone](#convex-cone)

In [conic optimization](convex-optimization.md#conic-optimization), a proper cone is a closed [convex cone](#convex-cone) that is a [pointed cone](#pointed-cone) and has nonempty interior in its ambient finite-dimensional space. These conditions permit strict cone feasibility and nondegenerate barrier geometry.

#### Completely positive cone

↑ **Parent:** [Convex cone](#convex-cone)

The [convex cone](#convex-cone) of [completely positive matrices](linear-algebra.md#completely-positive-matrix):

$$
\operatorname{CP}_n=\operatorname{cone}\{xx^T:x\in\mathbb R_{\geq0}^n\}.
$$

It is a [closed convex cone](#closed-convex-cone) and the [dual cone](toric-geometry.md#dual-cone) of the [copositive cone](#copositive-cone) under the [Frobenius inner product](linear-algebra.md#frobenius-inner-product). The finite-sum definition imposes no closure by fiat; [closedness of the completely positive cone](#closedness-of-the-completely-positive-cone) supplies that fact.

##### Closedness of the completely positive cone

↑ **Parent:** [Completely positive cone](#completely-positive-cone)

Use the [conic Carathéodory theorem](#conic-caratheodory-theorem) in the real space of [symmetric matrices](linear-algebra.md#symmetric-matrix), of [dimension](vector-space.md#dimension-vector-space) $N=n(n+1)/2$. A convergent sequence $B_\ell$ in the [completely positive cone](#completely-positive-cone) has padded factorizations $B_\ell=\sum_{j=1}^N x_{\ell j}x_{\ell j}^T$ with nonnegative factors. Their total squared norms equal $\operatorname{tr}B_\ell$ and are uniformly bounded. A simultaneous convergent subsequence of the finite factor tuple gives $B=\sum_jx_jx_j^T$ with $x_j\geq0$. Thus the limit remains in the cone. The argument also bounds the required number of factors by $N$.

#### Pointed cone

↑ **Parent:** [Convex cone](#convex-cone)

A [convex cone](#convex-cone) containing no nonzero line through the origin, equivalently $K\cap(-K)=\{0\}$. The [copositive cone](#copositive-cone) is pointed: a [matrix](vector-space.md#matrix) in both it and its negative has zero [quadratic form](linear-algebra.md#quadratic-form) on the [nonnegative orthant](#nonnegative-orthant); testing $e_i$ and $e_i+e_j$ kills all entries.

#### Closed convex cone

↑ **Parent:** [Convex cone](#convex-cone)

A [convex cone](#convex-cone) that is a [closed set](topology.md#closed-set) in its ambient topology. In a finite-dimensional [normed vector space](functional-analysis.md#normed-vector-space), this means it contains every limit of its convergent sequences. For example, the [positive semidefinite cone](#positive-semidefinite-cone) is closed because each test $X\mapsto x^TXx$ is continuous.

##### Separation from a closed convex cone

↑ **Parent:** [Closed convex cone](#closed-convex-cone)

For a [closed convex cone](#closed-convex-cone) $C$ in a finite-dimensional real [inner product](linear-algebra.md#inner-product) space and $z\notin C$, there exists $y$ with $\langle y,z\rangle<0$ and $\langle y,c\rangle\geq0$ for all $c\in C$. Here is a direct proof. A nearest point $c_0\in C$ exists by [compactness](topology.md#compact-space) after restricting to a sufficiently large ball. Differentiating squared distance along the segment towards $c\in C$ gives $\langle c_0-z,c-c_0\rangle\geq0$. Using $c=0$ and $c=2c_0$ shows $\langle c_0-z,c_0\rangle=0$. Set $y=c_0-z\ne0$: then $\langle y,c\rangle\geq0$ and $\langle y,z\rangle=-\|y\|^2<0$. This is a conic form of the [Hahn-Banach separation theorem](functional-analysis.md#hahn-banach-separation-theorem).

#### Conic hull

↑ **Parent:** [Convex cone](#convex-cone)

The set of all finite [conic combinations](#conic-combination) of elements of $S$, including zero. It is the smallest [convex cone](#convex-cone) containing $S$. It need not be closed even when $S$ is closed: the [closed set](topology.md#closed-set) $S=\{(t,1):t\geq1\}$ generates [vectors](vector-space.md#vector) converging to $(1,0)$ via $(t,1)/t$, but no nonzero generated [vector](vector-space.md#vector) has second coordinate zero.

##### Finitely generated cone

↑ **Parent:** [Conic hull](#conic-hull)

A [finitely generated cone](#finitely-generated-cone) is a [conic hull](#conic-hull) of a finite set of vectors. Every point admits a representation using linearly independent active generators, by eliminating dependence while keeping coefficients nonnegative.

###### Closedness of finitely generated cones

↑ **Parent:** [Finitely generated cone](#finitely-generated-cone)

A [finitely generated cone](#finitely-generated-cone) is a [closed convex cone](#closed-convex-cone). For a convergent sequence of represented vectors, use linearly independent active generators and pass to a subsequence with the same active set. Its coefficients converge through a fixed left inverse and retain nonnegativity. General linear images of closed cones need not be closed; finiteness of the generators supplies the missing argument.

##### Conic combination

↑ **Parent:** [Conic hull](#conic-hull)

A finite sum $\sum_j\lambda_js_j$ with $\lambda_j\geq0$. Unlike a [convex combination](#convex-combination), the [coefficients](vector-space.md#coefficient) need not sum to one. Zero [coefficients](vector-space.md#coefficient) and the empty sum are allowed.

#### Copositive cone

↑ **Parent:** [Convex cone](#convex-cone)

The real [symmetric matrices](linear-algebra.md#symmetric-matrix) that are [copositive matrices](linear-algebra.md#copositive-matrix) form a closed [convex cone](#convex-cone):

$$
\operatorname{COP}_n=\{A:x^TAx\geq0\text{ for every }x\in\mathbb R_{\geq0}^n\}.
$$

Each fixed $x$ gives a closed linear inequality in $A$. Their intersection is therefore closed and [convex](real-analysis.md#convex-function), and it is preserved by nonnegative scaling.

##### Duality of copositive and completely positive cones

↑ **Parent:** [Copositive cone](#copositive-cone)

Under the nonnegative-pairing convention for the [dual cone](toric-geometry.md#dual-cone), $\operatorname{CP}_n^*=\operatorname{COP}_n$ follows from $\langle A,xx^T\rangle_F=x^TAx$. Conversely, if $B\notin\operatorname{CP}_n$, [separation from a closed convex cone](#separation-from-a-closed-convex-cone) gives a separating $A$ nonnegative on all generators and negative on $B$. That $A$ is a [copositive matrix](linear-algebra.md#copositive-matrix), so $B\notin\operatorname{COP}_n^*$. This proves the displayed equality using [closedness of the completely positive cone](#closedness-of-the-completely-positive-cone).

##### Interior of the copositive cone

↑ **Parent:** [Copositive cone](#copositive-cone)

The [interior](topology.md#interior-topology) consists exactly of [strictly copositive matrices](linear-algebra.md#strictly-copositive-matrix). If $x^TAx$ has positive minimum $\delta$ on the [compact](topology.md#compact-space) nonnegative [unit sphere](topology.md#unit-sphere), perturbations of [operator norm](continuous-dual-space.md#operator-norm) less than $\delta$ preserve this positive lower bound there. Conversely, if a unit nonnegative [vector](vector-space.md#vector) has zero [quadratic form](linear-algebra.md#quadratic-form), $A-\varepsilon I$ leaves the [copositive cone](#copositive-cone) for every $\varepsilon>0$. Thus such a [matrix](vector-space.md#matrix) is not [interior](topology.md#interior-topology). The [identity matrix](vector-space.md#identity-matrix) is a convenient [interior](topology.md#interior-topology) point.

##### Positive-semidefinite-plus-nonnegative cone

↑ **Parent:** [Copositive cone](#copositive-cone)

The sums $P+N$ of a real [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) $P$ and a symmetric [nonnegative matrix](vector-space.md#nonnegative-matrix) $N$ form a [convex cone](#convex-cone) inside the [copositive cone](#copositive-cone). Both terms have nonnegative [quadratic forms](linear-algebra.md#quadratic-form) on the [nonnegative orthant](#nonnegative-orthant). The [Horn copositive matrix](linear-algebra.md#horn-copositive-matrix) shows that the inclusion is strict in dimension five; the [sum of squares criterion for a biquadratic form](polynomial.md#sum-of-squares-criterion-for-a-biquadratic-form) explains this cone's relation to [semidefinite programming](convex-optimization.md#semidefinite-programming).

#### Positive semidefinite cone

↑ **Parent:** [Convex cone](#convex-cone)

The positive semidefinite matrices form a convex cone because nonnegative combinations preserve nonnegative quadratic forms.

##### Elliptope

↑ **Parent:** [Positive semidefinite cone](#positive-semidefinite-cone)

The set of real [positive semidefinite matrices](linear-algebra.md#positive-semidefinite-matrix) with unit diagonal. Equivalently, its members are [Gram matrices](linear-algebra.md#gram-matrix) of unit [vectors](vector-space.md#vector), by the [real spectral theorem](linear-operator-theory.md#real-spectral-theorem). Every two-by-two [principal minor](vector-space.md#principal-minor) gives $|X_{ij}|\leq1$, so the set is bounded; it is also closed, hence [compact](topology.md#compact-space) in finite [dimension](vector-space.md#dimension-vector-space). This gives attainment of linear objectives used in [semidefinite programming](convex-optimization.md#semidefinite-programming).

##### Fantope

↑ **Parent:** [Positive semidefinite cone](#positive-semidefinite-cone)

For an integer $0\leq k\leq n$, the fantope is the [convex hull](#convex-hull) of rank-$k$ [orthogonal projection matrices](linear-algebra.md#orthogonal-projection-matrix) in $\mathbb R^n$. Equivalently, it consists of real [symmetric matrices](linear-algebra.md#symmetric-matrix) with [eigenvalues](linear-operator-theory.md#eigenvalue) in $[0,1]$ and [matrix trace](linear-algebra.md#matrix-trace) $k$. To prove the equivalence, apply the [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) and express the [eigenvalue](linear-operator-theory.md#eigenvalue) vector as a [convex combination](#convex-combination) of the zero-one [extreme points](#extreme-point) of the [capped simplex](#capped-simplex). The [sum of the largest eigenvalues](#sum-of-the-largest-eigenvalues) is its [support function](#support-function).

##### Trace constraint

↑ **Parent:** [Positive semidefinite cone](#positive-semidefinite-cone)

For a positive semidefinite matrix, a trace bound is a bound on the sum of its nonnegative eigenvalues.

###### Positive semidefinite trace ball

↑ **Parent:** [Trace constraint](#trace-constraint)

The positive semidefinite trace ball of radius $s$ is

$$
\mathcal S_s=\{Z=Z^T:Z\succeq0,\ \operatorname{tr}Z\leq s\}.
$$

It is closed and convex, and $\|Z\|_F\leq\operatorname{tr}Z\leq s$ for every $Z\in\mathcal S_s$.

###### Projection onto a positive semidefinite trace ball

↑ **Parent:** [Positive semidefinite trace ball](#positive-semidefinite-trace-ball)

If $M\succeq0$ has eigenpairs $(\mu_i,v_i)$ and $\operatorname{tr}M>s$, then its Frobenius projection onto $\mathcal S_s$ is

$$
\Pi_{\mathcal S_s}(M)
=\sum_i(\mu_i-\rho)_+v_iv_i^T,
$$

where $\rho>0$ is uniquely determined by $\sum_i(\mu_i-\rho)_+=s$.

## Game theory

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

[This section is present in another page, follow this link to view it.](game-theory.md)

## Mathematical finance

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

[This section is present in another page, follow this link to view it.](mathematical-finance.md)

## Positive-definite quadratic optimization

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)

A linear functional minus one half of a positive-definite quadratic has the unique maximizer obtained by solving its linear first-order equation.

### Orthogonal decomposition in a positive-definite metric

↑ **Parent:** [Positive-definite quadratic optimization](#positive-definite-quadratic-optimization)

A positive-definite matrix $V$ defines the inner product $x^TVy$, allowing decomposition into a chosen direction and its $V$-orthogonal complement.

## ↑ Ancestors (3)

1. [Area of mathematics](mathematics.md#area-of-mathematics)
2. [Mathematics](mathematics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Interior-point method](convex-optimization.md#interior-point-method)
- [Mathematical economics](mathematics.md#mathematical-economics)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37.md#4/solution)
- [Primal problem](#primal-problem)
