<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For subsets $A,B\subseteq\mathbb N$, a [many-one reduction](../../../../../many-one-reduction.md) $A\leq_m B$ is a [total computable function](../../../../../total-computable-function.md) $h$ with $n\in A\iff h(n)\in B$. A [Turing reduction](../../../../../turing-reduction.md) $A\leq_T B$ is an [oracle machine](../../../../../oracle-machine.md) with oracle $B$ computing the total [indicator function](../../../../../indicator-function.md) $\chi_A$. It may make several adaptive oracle queries. A [many-one reduction](../../../../../many-one-reduction.md) gives a [Turing reduction](../../../../../turing-reduction.md) using one query; the definitions impose no enumerability assumption on $A,B$.

The [Friedberg–Muchnik theorem](../../../../../friedberg-muchnik-theorem.md) asserts that there exist [computably enumerable sets](../../../../../recursively-enumerable-set.md) $A,B$ with

$$
\boxed{A\not\leq_T B\quad\text{and}\quad B\not\leq_T A.}
$$

We give the [finite-injury priority construction](../../../../../finite-injury-priority-construction.md). Fix an effective list $\Phi_e$ of [Turing functionals](../../../../../turing-functional.md) and impose

$$
R_e:\Phi_e^B\ne\chi_A,\qquad S_e:\Phi_e^A\ne\chi_B,
$$

in priority order $R_0,S_0,R_1,S_1,\ldots$. Each strategy has an unassigned, waiting or protected state; a private witness $x$ when assigned; and a restraint on the oracle [set](../../../../../set-split.md) when protected. All witnesses, even abandoned ones, are permanently recorded and never reused. A strategy for $R_e$ is the only strategy ever allowed to enumerate its witness into $A$; the analogous statement holds for $S_e$ and $B$.

Start with [finite sets](../../../../../finite-set.md) $A_0=B_0=\varnothing$. At stage $s$, inspect the first $s+1$ strategies. An unassigned strategy needs attention. A waiting $R_e$ strategy needs attention if the computation $\Phi_e^{B_s}(x)$ converges within $s$ steps; waiting $S_e$ is symmetric. Act on the highest-priority strategy needing attention, if any. On assignment choose a fresh witness greater than $s$, every earlier witness and every higher-priority restraint, and enter the waiting state. On a convergence with output $v$ and [oracle use](../../../../../oracle-use.md) $u$, act as follows: if $v=0$, enumerate the witness into its own target [set](../../../../../set-split.md); if $v\ne0$, leave the witness out. Enter the protected state and restrain the oracle below $u$. The current characteristic value at the witness is now different from $v$, including outputs other than zero or one. Whenever a strategy acts, initialize every lower-priority strategy, discarding its current witness and restraint but retaining the permanent record of used witnesses. If none needs attention, change nothing.

Every enumeration respects higher-priority restraints: its witness was chosen beyond them after its last initialization, and a later higher-priority action would have initialized it. Each stage is effective, finite and monotone in $A_s,B_s$, so $A=\bigcup_s A_s$ and $B=\bigcup_s B_s$ are computably enumerable. Lower-priority restraints may be violated by a higher-priority action, exactly the allowed injuries.

Induct on priority to verify [finite injury](../../../../../finite-injury.md) and satisfaction. Once all higher-priority strategies have made their last actions, the current strategy receives its final assignment and can act at most once more, on a convergence. If convergence is observed it is then protected permanently; otherwise it waits without further action. In either case every strategy acts only finitely often. After the final initialization of $R_e$, if it acts on a convergence, no higher strategy subsequently changes its assumptions and every lower strategy respects its restraint. The observed oracle computation therefore remains valid for the final $B$, while the permanently private witness retains the opposite characteristic value in $A$.

If it waits forever, then $\Phi_e^B(x)$ cannot converge. A convergent final computation uses only finitely many oracle bits; those bits in the increasing enumeration $B_s$ eventually equal their final values. For a sufficiently large stage the same finite computation would have been observed, and after the higher strategies have stopped it would receive attention, contradicting perpetual waiting. Thus $R_e$ is satisfied either by disagreement or by divergence. The same proof satisfies every $S_e$. This is [private-witness diagonalization for incomparable enumerable sets](../../../../../private-witness-diagonalization-for-incomparable-enumerable-sets.md), with the finite-injury verification supplying the required permanent disagreements.

A computable [set](../../../../../set-split.md) reduces to every oracle, so incomparability makes both [sets](../../../../../set-split.md) noncomputable. Every [computably enumerable set](../../../../../recursively-enumerable-set.md) reduces to the [halting problem](../../../../../halting-problem.md); if either of these [sets](../../../../../set-split.md) had the halting degree, the other would reduce to it. Thus their c.e. degrees are also incomplete, giving the intermediate degrees sought by the [Post problem](../../../../../post-problem.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
