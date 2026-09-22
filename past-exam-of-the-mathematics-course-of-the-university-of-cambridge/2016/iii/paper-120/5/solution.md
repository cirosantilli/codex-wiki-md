<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [many-one reduction](../../../../../many-one-reduction.md) $A\leq_m B$ is a [total computable function](../../../../../total-computable-function.md) $f:\mathbb N\to\mathbb N$ such that

$$
n\in A\quad\Longleftrightarrow\quad f(n)\in B.
$$

A [Turing reduction](../../../../../turing-reduction.md) $A\leq_TB$ is an [oracle machine](../../../../../oracle-machine.md) which, with membership oracle $B$, halts on every input and computes the [indicator function](../../../../../indicator-function.md) $\chi_A$. It may make finitely many adaptive queries on each input. A [many-one reduction](../../../../../many-one-reduction.md) gives a [Turing reduction](../../../../../turing-reduction.md) by a single query, but [Turing reducibility](../../../../../turing-reduction.md) allows more general procedures.

**The [Friedberg–Muchnik theorem](../../../../../friedberg-muchnik-theorem.md) states that there are [computably enumerable sets](../../../../../recursively-enumerable-set.md) $A,B$ with incomparable [Turing degrees](../../../../../turing-degree.md)**:

$$
\boxed{A\not\leq_TB\quad\text{and}\quad B\not\leq_TA.}
$$

Here is a [finite-injury priority construction](../../../../../finite-injury-priority-construction.md) proving it. Effectively enumerate all [Turing functionals](../../../../../turing-functional.md) $(\Phi_e)$. Arrange the requirements in the priority order

$$
R_0,S_0,R_1,S_1,\ldots,
\qquad R_e:\Phi_e^A\ne\chi_B,
\qquad S_e:\Phi_e^B\ne\chi_A.
$$

Equality would require the [Turing functional](../../../../../turing-functional.md) to be total and give the correct bit at every input; one disagreement or one undefined input defeats it.

Start with $A_0=B_0=\varnothing$ and enumerate elements without ever removing them. A strategy has a private witness, a flag recording whether it has acted, and a restraint on its oracle. Every new witness is larger than every previously assigned witness and every current higher-priority restraint. Retired witnesses are never reused. The only possible enumeration of a witness is by its owner, so an unacted witness remains outside its target set.

The strategy for $R_e$ chooses a witness $x$ and waits for a stage at which the bounded simulation gives

$$
\Phi_e^{A_s}(x)\downarrow=0.
$$

On seeing this, put $x$ into $B$, declare the strategy acted, and impose restraint $u$ on $A$, where $u$ is the [oracle use](../../../../../oracle-use.md): one more than the largest queried number, or zero if there were no queries. Initialize every lower-priority strategy, discarding its current witness, acted flag and restraint. An acted strategy does nothing further until initialized. The strategy for $S_e$ is identical with $A,B$ interchanged. Waiting specifically for zero is enough: if the eventual output is nonzero while the witness stays out, it already disagrees with the target [indicator function](../../../../../indicator-function.md).

For a completely effective schedule, at stage $s$ visit the first $s+1$ strategies in priority order. Assign an unassigned witness when visited. Simulate each unacted strategy's computation for at most $s$ steps with the current finite oracle. If some strategy can act, perform the first such action and end the stage; otherwise end after all visits. All steps are finite and algorithmic, so the limiting $A,B$ are [computably enumerable sets](../../../../../recursively-enumerable-set.md).

Every lower-priority enumeration respects higher-priority restraints. When its witness was chosen it lay above these restraints. Any subsequent action of a higher-priority strategy would have initialized it, so its current witness remains safe to enumerate. The initialization of all lower strategies also removes their obsolete restraints before they can obstruct a legitimate higher-priority action.

We verify [finite injury](../../../../../finite-injury.md) by [mathematical induction](../../../../../mathematical-induction.md) on priority. The first strategy is never injured and acts at most once. If all predecessors of a strategy act finitely often, there is a last stage when a higher-priority action initializes it. It is subsequently visited, chooses its permanent witness, and acts at most once. Thus it too acts finitely often and all its lower-priority strategies suffer only finitely many injuries. The scheduling cannot starve a fixed strategy: after the finitely many higher-priority actions, all sufficiently large stages visit it.

Consider the final uninjured $R_e$ with witness $x$. If it acts, then $x\in B$ permanently, and every later lower-priority enumeration into $A$ respects its restraint. No later higher-priority action occurs. The preserved computation is therefore

$$
\Phi_e^A(x)=0\ne1=\chi_B(x).
$$

If it never acts, $x\notin B$. Were $\Phi_e^A=\chi_B$, the final computation on $x$ would halt with zero and have finite [oracle use](../../../../../oracle-use.md). The finitely many oracle bits it queries eventually stabilize, and a sufficiently late bounded stage simulation would see exactly this zero computation. The strategy would then act, a contradiction. Hence $R_e$ holds in this case too. The same reasoning proves every $S_e$.

All possible [Turing reductions](../../../../../turing-reduction.md) in both directions are excluded. This proves the [Friedberg–Muchnik theorem](../../../../../friedberg-muchnik-theorem.md); in particular both constructed [Turing degrees](../../../../../turing-degree.md) are noncomputable, since a [computable set](../../../../../computable-set.md) is [Turing reducible](../../../../../turing-reduction.md) to every oracle.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
