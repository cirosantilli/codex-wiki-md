<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [many-one reduction](../../../../../many-one-reduction.md) $A\leq_mB$ is a [total computable function](../../../../../total-computable-function.md) $f$ with $x\in A\iff f(x)\in B$. A [Turing reduction](../../../../../turing-reduction.md) $A\leq_TB$ is an [oracle machine](../../../../../oracle-machine.md) which decides $A$ with oracle $B$. It may make several adaptive queries and combine their answers. Every many-one reduction is a Turing reduction, by asking the single question $f(x)\in B$. The converse fails: for the [diagonal halting set](../../../../../diagonal-halting-set.md) $K$, its complement is Turing-reducible to $K$ by reversing one oracle answer, but is not many-one reducible to $K$. Such a reduction would make the complement [computably enumerable](../../../../../recursively-enumerable-set.md), contradicting undecidability of the [halting problem](../../../../../halting-problem.md).

The [Friedberg–Muchnik theorem](../../../../../friedberg-muchnik-theorem.md) asserts that there are [computably enumerable sets](../../../../../recursively-enumerable-set.md) $A,B$ with incomparable [Turing degrees](../../../../../turing-degree.md):

$$
\boxed{A\not\leq_TB\quad\text{and}\quad B\not\leq_TA.}
$$

Here is a [finite-injury priority construction](../../../../../finite-injury-priority-construction.md) proving it. Enumerate all [Turing functionals](../../../../../turing-functional.md) $\Phi_e$ and put the requirements in the priority order

$$
R_0>S_0>R_1>S_1>\cdots,\qquad
R_e:\Phi_e^B\ne\chi_A,\quad S_e:\Phi_e^A\ne\chi_B.
$$

Start with $A_0=B_0=\varnothing$. Each requirement has a fresh witness, a waiting or acted status, and a restraint on the other set. A restraint $u$ forbids lower-priority strategies from enumerating numbers below $u$ into that oracle. Globally remember all previously chosen witnesses, including abandoned ones, and never choose any of them again.

For $R_e$, choose an unused witness $x$ outside $A_s\cup B_s$, larger than the stage and every current higher-priority restraint. Keep it out of $A$. Wait until the bounded simulation $\Phi_{e,s}^{B_s}(x)$ converges with value zero. If this happens, enumerate $x$ into $A$, put a restraint $u$ on $B$, where $u$ is one more than the largest oracle query in the observed computation, and mark the strategy acted. For $S_e$, interchange $A$ and $B$.

At stage $s$, consider the first $s+1$ requirements. Choose the highest-priority one needing a witness or waiting with an observed zero computation. Perform its indicated action, then initialize all lower-priority requirements: abandon their witnesses, clear their restraints, and reset their status. Do nothing if no requirement needs attention. Since witness selection respects higher restraints, and higher actions initialize every lower strategy, all protected computations are respected by lower-priority enumerations. Each stage is a finite effective calculation, so $A=\bigcup_sA_s$ and $B=\bigcup_sB_s$ are [computably enumerable sets](../../../../../recursively-enumerable-set.md).

Verify by induction along the priority order that every requirement is initialized only finitely often and acts only finitely often. The highest requirement chooses one witness and can diagonalize at most once. After all higher requirements have finished acting, the next requirement is never again initialized; it obtains a final witness and can diagonalize at most once. This proves [finite injury](../../../../../finite-injury.md) for every requirement and ensures that no requirement is permanently starved by higher attention.

Consider $R_e$ after its last initialization. If it acts, its witness belongs to $A$, while the protected computation with oracle $B$ remains zero: higher strategies no longer act and lower ones respect its restraint. Thus $\Phi_e^B(x)\ne\chi_A(x)$. If it never acts, its private witness remains outside $A$. Were $\Phi_e^B=\chi_A$, the computation on that witness would converge to zero with a finite [oracle use](../../../../../oracle-use.md). Since the increasing sets $B_s$ eventually agree with $B$ on this finite initial segment, a sufficiently late bounded simulation would detect that computation and make $R_e$ act, a contradiction. The symmetric argument verifies every $S_e$.

Thus the two sets have incomparable Turing degrees. Both are noncomputable, since a computable set is Turing-reducible to every oracle. Both are also strictly below the degree of the [halting problem](../../../../../halting-problem.md): every computably enumerable set is Turing-reducible to $K$, while completeness of one would make the other reducible to it. This supplies the intermediate degrees sought in [Post problem](../../../../../post-problem.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
