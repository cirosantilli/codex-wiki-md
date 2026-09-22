<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $t_k\in\{0,1\}$ encode the truth value of $X_k$. For a [Boolean literal](../../../../../boolean-literal.md) $\ell$, write $L_\ell(t)=t_k$ if $\ell=X_k$ and $L_\ell(t)=1-t_k$ if $\ell=\overline X_k$. A clause is true precisely when the sum of its literal values is at least one. Thus the [integer programming formulation of satisfiability](../../../../../integer-programming-formulation-of-satisfiability.md) is the feasibility problem

$$
\boxed{t_k\in\{0,1\},\qquad \sum_{j=1}^{M_i}L_{x_{ij}}(t)\geq1\quad(1\leq i\leq N),}
$$

with objective zero. Every feasible binary vector gives a satisfying assignment of the [Boolean satisfiability problem](../../../../../boolean-satisfiability-problem.md), and conversely. An empty clause gives $0\geq1$ and hence infeasibility.

For [maximum satisfiability](../../../../../maximum-satisfiability.md), introduce binary variables $q_i$ marking clauses selected as satisfied and solve

$$
\boxed{\max\sum_{i=1}^Nq_i,\qquad t_k,q_i\in\{0,1\},\qquad q_i\leq\sum_{j=1}^{M_i}L_{x_{ij}}(t)\quad(1\leq i\leq N).}
$$

A false clause forces $q_i=0$, while a true clause permits $q_i=1$. At an optimum every permitted $q_i$ is one, since increasing it improves the objective without affecting another constraint. Therefore the objective is exactly the maximum number of simultaneously true clauses. Repeated literals cause no difficulty, and a clause containing both signs of a variable is always true.

For the [literal-frequency greedy approximation for MAX-SAT](../../../../../literal-frequency-greedy-approximation-for-max-sat.md), keep only clauses not already satisfied and remove literals made false. Count occurrence in clauses, rather than multiplicity within a clause. At a step let $a$ be the number of current clauses containing the chosen literal $z$, and $b$ the number containing its opposite $\overline z$. Since $z$ has maximum clause frequency among all remaining literals, $b\leq a$.

Setting $z$ true permanently satisfies exactly the $a$ clauses containing it. Some other clauses may become empty and are then permanently lost. Every newly empty clause previously contained $\overline z$, so their number $d$ satisfies

$$
d\leq b\leq a.
$$

A clause containing both signs is satisfied and cannot be one of the lost clauses. Repeat this accounting at every step. Satisfied clauses are removed, so no success is counted twice; each lost nonempty original clause becomes empty at exactly one step. If $G$ is the total number satisfied and $D$ the number of initially nonempty clauses lost, summing the inequalities gives $D\leq G$. Every initially nonempty clause eventually falls into one of these two classes. Writing their number as $N_+$, we get

$$
G+D=N_+,\qquad G\geq N_+/2.
$$

Even an optimal assignment can satisfy at most $N_+$ clauses. Consequently

$$
\boxed{G\geq\frac12N_+\geq\frac12\operatorname{OPT}.}
$$

Thus Greedy is a $1/2$-approximation in the convention stated in the question. The proof also covers initial empty clauses by excluding them from $N_+$; they are unsatisfiable for every algorithm.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
