<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [integer program](../../../../../integer-programming.md) for the [travelling salesman problem](../../../../../travelling-salesman-problem.md) must exclude disconnected cycle covers, not merely require one incoming and one outgoing edge. Here is a [compact order formulation of the travelling salesman problem](../../../../../compact-order-formulation-of-the-travelling-salesman-problem.md). The one-city case is trivial. For $n\geq2$, use binary variables $x_{ij}$ for directed edges, $i\ne j$, and integer variables $u_i$ for $i=2,\ldots,n$. Minimize $\sum_{i\ne j}d_{ij}x_{ij}$ subject to

$$
\begin{gathered}
\sum_{j\ne i}x_{ij}=1,\qquad\sum_{j\ne i}x_{ji}=1\quad(1\leq i\leq n),\\
0\leq x_{ij}\leq1,\qquad1\leq u_i\leq n-1,\\
u_i-u_j+(n-1)x_{ij}\leq n-2\quad(2\leq i\ne j\leq n).
\end{gathered}
$$

The degree equations give a collection of disjoint directed cycles. Along any selected edge between nondistinguished cities, the last inequality gives $u_j\geq u_i+1$. Summing around a cycle avoiding city $1$ would yield $0\geq k$ for its positive length $k$. Thus every cycle must contain city $1$, so there is exactly one tour. Conversely, number the cities after city $1$ in tour order, giving $u_i\in\{1,\ldots,n-1\}$. Selected edges satisfy the order inequalities. Unselected edges impose no additional restriction, since $u_i-u_j\leq n-2$. This proves equivalence with tours, including symmetric-distance instances represented by directed variables.

There are $O(n^2)$ variables and rows. For the bit count, store only nonzero coefficients and their indices. The degree equations have $O(n^2)$ entries in total; each order inequality has three entries, so these too have $O(n^2)$ entries. Indices and the coefficients bounded by $n$ need $O(\log n)$ bits each. The objective has $O(n^2)$ distance coefficients, each needing at most $n+1$ bits because the PDF's bound is $2^n$. Therefore

$$
\boxed{\text{sparse ILP encoding length}=O(n^3).}
$$

Writing an unnecessarily dense constraint matrix would give a larger encoding; it is the sparse explicit encoding that establishes the requested bound. For the decision version add $\sum d_{ij}x_{ij}\leq B$. A threshold can be capped at $n2^n$, so its relevant binary length is $O(n+\log n)$; negative thresholds can be rejected immediately for nonnegative distances.

A decision problem belongs to [NP](../../../../../np-complexity.md) if its yes-instances have certificates of polynomial length checkable in deterministic polynomial time. It is [NP-complete](../../../../../np-completeness.md) if it belongs to NP and every NP problem has a [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) to it. The preceding construction is a polynomial-time reduction from travelling-salesman decision to integer-linear feasibility. If the former is NP-complete, the latter is consequently NP-hard.

For completeness we must also establish membership in NP for general integer-linear feasibility, rather than just for the binary instances produced by the reduction. An arbitrary feasible integer assignment could be numerically enormous; what is needed is the existence of a short one. We give a [small integer feasibility witness by homogeneous cone decomposition](../../../../../small-integer-feasibility-witness-by-homogeneous-cone-decomposition.md).

Split each unrestricted integer variable into the difference of two nonnegative integer variables and add nonnegative integer slacks to inequalities. This gives $Bz=b$, $z\geq0$, with $N$ variables and integer data bounded in absolute value by $M\geq1$. Both $N$ and $\log M$ are polynomially bounded by the original input length. Consider the homogeneous cone

$$
K=\{(u,t)\geq0:Bu=bt\}\subseteq\mathbb R^{N+1}.
$$

Every vector in this cone is a nonnegative combination of at most $N+1$ support-minimal rays. To prove this, choose a nonnegative kernel vector $h$ of minimal nonempty support contained in the support of a given vector, subtract $\lambda h$ with $\lambda$ the smallest positive coordinate ratio, and repeat. Each subtraction strictly reduces support. On a minimal support the kernel is one-dimensional: an independent kernel direction would let us perturb a positive vector to the boundary of its support without making it zero, contradicting minimality. Cofactors of independent rows therefore give an integer nonnegative generator of each such ray. Every coordinate is bounded by

$$
D=(N+1)!M^{N+1},
$$

using the elementary determinant bound. This proves the needed [support-minimal rays of a nonnegative kernel](../../../../../support-minimal-rays-of-a-nonnegative-kernel.md) facts directly.

Start with any integer feasible $z$ and decompose $(z,1)$ in this way. A ray whose last coordinate is a positive integer $q$ normalizes to a point $v$ with $Bv=b$ and $0\leq v_i\leq D$; the coefficients of these normalized points sum to one. Rays with last coordinate zero have integer nonnegative first coordinates $r_j$ with $Br_j=0$ and coordinates at most $D$. Hence

$$
z=\sum_k\lambda_kv_k+\sum_jt_jr_j,\qquad\lambda_k\geq0,\quad\sum_k\lambda_k=1,\quad t_j\geq0,
$$

with at most $N+1$ ray terms. Subtract $\sum_j\lfloor t_j\rfloor r_j$ from $z$. The result $z'$ is still integer, nonnegative and feasible, and satisfies

$$
0\leq z'_i\leq D+(N+1)D=(N+2)D.
$$

Its binary length is polynomial, since $\log D=O(N\log N+N\log M)$. The assignment can be checked by exact integer arithmetic in polynomial time. Thus general integer-linear feasibility is in NP. Combining this with the reduction proves

$$
\boxed{\text{TSP decision NP-complete}\ \Longrightarrow\ \text{ILP decision NP-complete}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
