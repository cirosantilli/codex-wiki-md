<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Use an [exactly-one constraint](../../../../../exactly-one-constraint.md) for each finite-domain [variable](../../../../../variable-mathematics.md) and a [Boolean clause](../../../../../clause-of-a-boolean-formula.md) forbidding each disallowed constraint tuple.** Let the [variables](../../../../../variable-mathematics.md) be $X_1,\ldots,X_n$, with explicitly listed finite [constraint domains](../../../../../constraint-domain.md) $D_i$, and let constraint $C$ have distinct-variable scope $S_C$ and allowed relation $R_C\subseteq\prod_{i\in S_C}D_i$. Introduce a [Boolean variable](../../../../../boolean-variable.md) $p_{i,v}$ for every $v\in D_i$, interpreted as $X_i=v$. The [direct SAT encoding of finite-domain constraints](../../../../../direct-sat-encoding-of-finite-domain-constraints.md) is

$$
\varphi_P=
\bigwedge_i\left[
\left(\bigvee_{v\in D_i}p_{i,v}\right)
\land
\bigwedge_{\{u,v\}\subseteq D_i,\ u\ne v}
(\neg p_{i,u}\lor\neg p_{i,v})
\right]
\land
\bigwedge_C\ \bigwedge_{\mathbf t\in F_C}
\left(\bigvee_{i\in S_C}\neg p_{i,t_i}\right),
\qquad F_C=\left(\prod_{i\in S_C}D_i\right)\setminus R_C.
$$

In the middle [logical conjunction](../../../../../logical-conjunction.md), each unordered distinct pair is included once. The first [Boolean clause](../../../../../clause-of-a-boolean-formula.md) requires at least one value, the pairwise [Boolean clauses](../../../../../clause-of-a-boolean-formula.md) permit at most one, and a final [Boolean clause](../../../../../clause-of-a-boolean-formula.md) is false exactly when all coordinates of one forbidden tuple are selected. The formula is in [conjunctive normal form](../../../../../conjunctive-normal-form.md). An empty [constraint domain](../../../../../constraint-domain.md) produces an empty [Boolean clause](../../../../../clause-of-a-boolean-formula.md), correctly making the instance unsatisfiable.

For soundness of the reduction, a solution $x$ of the [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md) gives the [Boolean valuation](../../../../../boolean-valuation.md) $p_{i,v}=1$ exactly when $v=x_i$. Every [exactly-one constraint](../../../../../exactly-one-constraint.md) holds; a forbidden tuple differs from $x$ on at least one scoped coordinate, making its negative [Boolean clause](../../../../../clause-of-a-boolean-formula.md) true. Thus $x$ supplies a [satisfying assignment](../../../../../satisfying-assignment.md) for $\varphi_P$.

Conversely, a [satisfying assignment](../../../../../satisfying-assignment.md) selects a unique value $x_i$ for every $X_i$. If a constraint failed, the selected scoped tuple would belong to $F_C$, and its entire negative [Boolean clause](../../../../../clause-of-a-boolean-formula.md) would be false. That contradicts satisfiability. Hence $x$ is a solution. Decoding takes $O(\sum_i|D_i|)$ by scanning the value indicators. This proves **$P$ has a solution if and only if $\varphi_P$ is satisfiable**.

For explicit size accounting, put $q_i=|D_i|$, $r_C=|S_C|$ and $f_C=|F_C|$. There are $\sum_iq_i$ [Boolean variables](../../../../../boolean-variable.md),

$$
K=n+\sum_i\binom{q_i}{2}+\sum_Cf_C
$$

[Boolean clauses](../../../../../clause-of-a-boolean-formula.md), and

$$
L=\sum_iq_i+2\sum_i\binom{q_i}{2}+\sum_Cr_Cf_C
$$

[literal](../../../../../boolean-literal.md) occurrences. These formulas count nonempty scopes; a false zero-arity constraint contributes an empty [Boolean clause](../../../../../clause-of-a-boolean-formula.md), while a true one contributes none. Formula storage is $O(K+L)$ [literal](../../../../../boolean-literal.md)-sized records; a bit-level encoding also stores indicator indices. With maximum [constraint domain](../../../../../constraint-domain.md) size $q$, $m$ constraints and maximum arity $r$, this is bounded by $O(nq^2+mrq^r)$ for nontrivial domains and scopes. In the common binary case it is **$O((n+m)q^2)$**.

The input representation matters: listing all forbidden tuples costs up to $\prod_{i\in S_C}q_i$ tests per constraint. This is polynomial for bounded arity and explicitly represented domains, but can be exponential in the description length of a succinct high-arity constraint. The translation is valid in that case without constituting a polynomial-size reduction. If a compact constraint is supplied as a polynomial-size [Boolean circuit](../../../../../boolean-circuit.md), one may instead encode that circuit using auxiliary [Boolean variables](../../../../../boolean-variable.md) and local [conjunctive normal form](../../../../../conjunctive-normal-form.md) equivalences, with size proportional to the circuit. No compact representation is silently assumed.

For the instance in (c), after unary filtering there are $17$ indicators. The five at-least-one [Boolean clauses](../../../../../clause-of-a-boolean-formula.md), $22$ pairwise at-most-one [Boolean clauses](../../../../../clause-of-a-boolean-formula.md) and $24$ forbidden-equality [Boolean clauses](../../../../../clause-of-a-boolean-formula.md) give **$51$ [Boolean clauses](../../../../../clause-of-a-boolean-formula.md)**. Setting only $p_{a,1},p_{b,2},p_{c,3},p_{d,2},p_{e,1}$ true encodes the displayed solution.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
