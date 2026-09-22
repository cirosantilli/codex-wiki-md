<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Treat the condition as another instruction operand. At issue, capture the tag or value of the particular older [processor condition flags](../../../../../processor-condition-flag.md) that the instruction reads. Later flag writers must not redirect that dependence. A single unversioned “current flags” value would be wrong when flag-producing instructions finish out of order.

**Without a reorder buffer.** A conservative implementation keeps the conditional instruction in its [reservation station](../../../../../reservation-station.md) until its predicate and required data operands are ready. If the predicate is true, send the instruction to its [functional unit](../../../../../functional-unit.md); if false, suppress its specified changes. Independent unconditional instructions in other [reservation stations](../../../../../reservation-station.md) can execute meanwhile, which already gives the overlap in part (c). A conditional [store instruction](../../../../../store-instruction.md) must not write [computer memory](../../../../../computer-memory-split.md) while its predicate is unresolved, and a false condition must not raise an exception associated with executing the suppressed operation.

[Register renaming](../../../../../register-renaming.md) makes the false case more subtle than simply throwing away an instruction. For a conditional update of destination `r2`, let $v_{\rm old}$ be its preceding logical value and let $v_{\rm calc}$ be the computed new value. The required result is

$$
\boxed{v_{\rm out}=\begin{cases}v_{\rm calc},&\text{predicate true},\\v_{\rm old},&\text{predicate false}.\end{cases}}
$$

If issue has already assigned a producer tag to the conditional instruction's destination, younger consumers wait for that tag in either case. Record the old destination as an additional input before changing its [register renaming](../../../../../register-renaming.md) map. When the predicate is false, broadcast $v_{\rm old}$ under the conditional instruction's new tag, or provide an equivalent correctly ordered mapping/merge mechanism. Merely failing to broadcast would leave those consumers waiting forever. Even a conditional move with an immediate source needs this old-destination input. A conditional instruction that sets [processor condition flags](../../../../../processor-condition-flag.md) needs the same preserve-or-replace treatment for the flags.

**With a reorder buffer.** Allocate a [reorder buffer](../../../../../reorder-buffer.md) entry at issue and use its tag, or a corresponding [physical register](../../../../../physical-register.md), as the persistent destination. The [CPU](../../../../../central-processing-unit.md) may use the same wait-for-predicate policy. It may also execute a candidate result early, retaining it and any exception privately in the [reorder buffer](../../../../../reorder-buffer.md) until the predicate is known. The [functional unit](../../../../../functional-unit.md) and possibly the [reservation station](../../../../../reservation-station.md) can then be released while the entry waits. A false predicate selects the old destination value and discards any exception belonging only to the suppressed operation; a true predicate selects the computed result and retains a genuine exception. [Instruction retirement](../../../../../instruction-retirement.md) changes architectural state only when the entry reaches the head and its predicate and status are resolved. [Store instructions](../../../../../store-instruction.md) similarly hold their writes until authorized [instruction retirement](../../../../../instruction-retirement.md).

A [reorder buffer](../../../../../reorder-buffer.md) by itself does not remove the destination ambiguity. For instance, a younger addition consuming `r2` must not irreversibly use $v_{\rm calc}$ if the predicate might be false. It can wait for the merged $v_{\rm out}$. A more aggressive design can predict the predicate, forward the predicted value and replay or squash dependent instructions if that prediction fails, using the [reorder buffer](../../../../../reorder-buffer.md) and saved [register renaming](../../../../../register-renaming.md) state for recovery.

**Performance comparison.** Let the predicate be available at time $L$, the candidate's ordinary source data at time $D$, and its [functional unit](../../../../../functional-unit.md) take $F$ cycles. Ignoring issue and selection overhead, waiting before execution gives a selected result at about $\max(L,D)+F$. Early execution into a [reorder buffer](../../../../../reorder-buffer.md) can give it at $\max(L,D+F)$, provided the old value is also ready when needed. For $D=0$, $L=50$ and $F=20$, that is $70$ versus $50$ cycles. Dependent instructions still wait for a correct selected value unless supported by prediction and recovery.

A [reorder buffer](../../../../../reorder-buffer.md) can therefore overlap useful candidate work with predicate computation and release scarce scheduling resources earlier, at the cost of buffered results and possible wasted execution. [Instruction retirement](../../../../../instruction-retirement.md) can still wait behind an older incomplete instruction. A design without a [reorder buffer](../../../../../reorder-buffer.md) could also retain a harmless early arithmetic result in its [reservation station](../../../../../reservation-station.md) until the predicate is ready, but it occupies that station longer and still must defer effects and exceptions. **The fundamental requirements are versioned predicate dependence, preservation of false-case values, and controlled commitment; the reorder buffer makes speculative completion and recovery more systematic.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
