<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For sets $A,B\subseteq\mathbb N$, [many-one reducibility](../../../../../many-one-reduction.md) means there is a [total computable function](../../../../../total-computable-function.md) $h$ such that

$$
A\leq_mB\quad\Longleftrightarrow\quad(\exists h\text{ total computable})(\forall x)\,[x\in A\Longleftrightarrow h(x)\in B].
$$

[Turing reducibility](../../../../../turing-reduction.md) $A\leq_TB$ means that a [Turing machine](../../../../../turing-machine.md) with oracle $B$ computes the [indicator function](../../../../../indicator-function.md) $\chi_A$, halting on every input. A [many-one reduction](../../../../../many-one-reduction.md) supplies a [Turing reduction](../../../../../turing-reduction.md) by computing $h(x)$ and making one membership query, so $A\leq_mB$ implies $A\leq_TB$.

The [Friedberg–Muchnik theorem](../../../../../friedberg-muchnik-theorem.md) states that **there are [computably enumerable sets](../../../../../recursively-enumerable-set.md) $A,B$ with $A\not\leq_TB$ and $B\not\leq_TA$**. We prove this by a [finite-injury priority construction](../../../../../finite-injury-priority-construction.md). Fix an effective enumeration $(\Phi_e)$ of the oracle [Turing functionals](../../../../../turing-functional.md) and arrange the requirements in the order

$$
R_0,S_0,R_1,S_1,\ldots,\qquad R_e:\Phi_e^B\ne\chi_A,\quad S_e:\Phi_e^A\ne\chi_B.
$$

A requirement owns a private witness, a success flag and a [priority restraint](../../../../../priority-restraint.md) on its oracle set. All witnesses ever chosen are distinct. An $R_e$ witness $x$ is reserved outside $A$, and only $R_e$ may enumerate that number into $A$; an $S_e$ witness is treated symmetrically. A [priority restraint](../../../../../priority-restraint.md) $r$ forbids lower-priority requirements from adding numbers less than $r$ to the specified oracle set. Initializing a requirement abandons its witness, clears its success flag and sets its [priority restraint](../../../../../priority-restraint.md) to zero; enumeration into $A$ or $B$ is never undone.

At stage $s$ consider the first $s+1$ requirements and serve the highest-priority one requiring attention. An unsuccessful requirement requires attention if it has no witness, or its current witness has a stage-$s$ oracle computation with output zero, found within $s$ steps. If there is no such requirement, do nothing. When a requirement with no witness is served, choose a fresh number larger than $s$, all previously chosen witnesses and all current higher-priority [priority restraints](../../../../../priority-restraint.md). When an $R_e$ with a witness $x$ and observed computation $\Phi_e^{B_s}(x)=0$ is served, enumerate $x$ into $A$, mark it successful, and restrain $B$ below the use of that computation. The use is one more than the largest queried oracle position, or zero if there were no queries. An $S_e$ acts in exactly the same way with $A,B$ interchanged. After either kind of service, initialize every currently assigned lower-priority requirement; the remaining lower priorities are already in their initial state.

This is an effective stage construction with finite sets $A_s,B_s$, and $A=\bigcup_sA_s$, $B=\bigcup_sB_s$ are [computably enumerable](../../../../../recursively-enumerable-set.md). Every enumeration respects all higher-priority [priority restraints](../../../../../priority-restraint.md): its private witness was selected above them, and any later service to a higher-priority requirement would have initialized it before it could act. We do not need to restrain a computation whose output is nonzero; a persistent nonzero output already disagrees with an unenumerated witness.

We verify the [finite injury](../../../../../finite-injury.md) assertion by induction along the priority order. After the last service to requirements above a fixed requirement $Q$, the requirement $Q$ is never initialized again. It can be served at most twice thereafter, once to choose its final witness and once to diagonalize. Whenever it needs attention it is eventually served, since the higher-priority requirements have ceased acting and each later stage considers a longer initial segment. Thus $Q$ has a final witness and makes only finitely many actions; this proves the induction and justifies the assumed last service above it.

For a final $R_e$ witness $x$, if the diagonalization occurs then $\chi_A(x)=1$, while [preservation of a restrained oracle computation](../../../../../preservation-of-a-restrained-oracle-computation.md) applies: its zero computation is preserved permanently because higher priorities no longer act and lower priorities respect the [priority restraint](../../../../../priority-restraint.md). Thus $\Phi_e^B(x)=0\ne\chi_A(x)$. If it never occurs, then $\chi_A(x)=0$. Were $\Phi_e^B(x)=0$, that convergent computation would use finitely many oracle answers. Because $B_s$ increases to $B$, those finitely many answers eventually stabilize, and a sufficiently late stage would discover the zero computation and cause diagonalization. This contradicts its never occurring. So in this case $\Phi_e^B(x)$ is undefined or nonzero and again disagrees with $\chi_A$. The identical argument verifies every $S_e$.

All the requirements hold, proving the theorem. Both sets are noncomputable: a computable set is [Turing reducible](../../../../../turing-reduction.md) to every oracle. Moreover, every [computably enumerable set](../../../../../recursively-enumerable-set.md) is [Turing reducible](../../../../../turing-reduction.md) to the [diagonal halting set](../../../../../diagonal-halting-set.md) $K$, and neither $A$ nor $B$ can have its [Turing degree](../../../../../turing-degree.md), since that would make it compute the other set. Hence

$$
\boxed{0<\deg_T(A),\deg_T(B)<0',\qquad\deg_T(A)\text{ and }\deg_T(B)\text{ are incomparable}.}
$$

This also gives many-one incomparability and answers the existence of intermediate [computably enumerable](../../../../../recursively-enumerable-set.md) [Turing degrees](../../../../../turing-degree.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
