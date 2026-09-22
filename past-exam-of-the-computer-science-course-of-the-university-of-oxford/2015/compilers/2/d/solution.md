<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [mathematical induction](../../../../../mathematical-induction.md) on the sequence of call and return events. The invariant concerns the [static chain](../../../../../static-chain.md) of the currently executing activation: every [stack frame](../../../../../stack-frame.md) on that chain is the most recent surviving activation of the procedure it represents. It need not hold for the saved chain of an arbitrary suspended caller while a recursive callee is running.

Initially only `main` is active, so the claim holds. Suppose it holds just before a direct call to a procedure $R$, whose lexical parent is $P$. Without [procedural parameters](../../../../../procedural-parameter.md), visibility of $R$ means that its declaration lies in the current procedure or in a lexically enclosing procedure. Therefore the activation of $P$ needed for the call is on the caller's [static chain](../../../../../static-chain.md). By the [induction hypothesis](../../../../../induction-hypothesis.md), it is the newest surviving activation of $P$.

Create a new activation of $R$ whose [static link](../../../../../static-link.md) points to this $P$ activation. The inherited chain is a suffix of the caller's chain, so its [stack frames](../../../../../stack-frame.md) still represent the newest surviving activations of their procedures. Adding $R$ does not make any of those inherited activations out of date: $R$ cannot be its own lexical ancestor. The new $R$ activation itself is plainly the newest activation of $R$. This covers recursive calls too: an older activation of $R$ may survive on the [dynamic chain](../../../../../dynamic-chain.md), but is absent from the new activation's [static chain](../../../../../static-chain.md).

On return, the callee and every call it made have finished. The caller's saved [stack frame](../../../../../stack-frame.md) and [static chain](../../../../../static-chain.md) are restored. Any temporarily newer activation of a procedure represented on that chain has returned, so each restored activation is again the most recent surviving one. Thus return preserves the invariant as well.

**The claim holds for the executing procedure's [static chain](../../../../../static-chain.md) throughout every execution using direct calls under [lexical scope](../../../../../lexical-scope.md).** Equivalently, writing $P_F$ for the procedure represented by a [stack frame](../../../../../stack-frame.md) $F$,

$$
\boxed{F\in\mathrm{staticChain}_{\mathrm{executing}}\ \Longrightarrow\ F=\mathrm{newestSurviving}(P_F).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
