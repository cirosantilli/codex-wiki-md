<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let `expr(e)` generate [postfix code](../../../../../postfix-code.md) that evaluates a [program expression](../../../../../program-expression.md) once, leaving one value above an otherwise unchanged evaluation [stack](../../../../../stack-data-structure.md). Let `stmt(s)` preserve the evaluation [stack](../../../../../stack-data-structure.md)'s height. Use `EQ` to pop two [integers](../../../../../integer-split.md) and push their [Boolean](../../../../../boolean-data-type.md) [equality](../../../../../equality-mathematics.md) result; `JZ L` pops that result and jumps to `L` when it is false. `JMP` is unconditional. All labels returned by `fresh()` are distinct, including labels inside recursively generated bodies.

```
generateCase(Case(control, arms)):
    done := fresh()
    emit expr(control)
    for (labelExpression, body) in arms, in source order:
        next := fresh()
        emit DUP
        emit expr(labelExpression)
        emit EQ
        emit JZ next
        emit POP
        emit stmt(body)
        emit JMP done
        emit LABEL next
    emit POP
    emit LABEL done
```

To verify the [stack invariant](../../../../../stack-invariant.md), write the incoming evaluation [stack](../../../../../stack-data-structure.md) as $sigma$. Immediately before any label test it is $sigma,v$, where $v$ is the controlling value. `DUP`, evaluation of the label with value $w$, and `EQ` change this to $sigma,v,[v=w]$. `JZ` removes the [Boolean](../../../../../boolean-data-type.md). On failure the surviving $v$ is available for the next label; on success `POP` removes it before the body runs. The body therefore starts and ends with $sigma$ and jumps past every remaining label. If every label fails, the final `POP` restores $sigma$.

**The controlling expression is evaluated once, each reached label is evaluated once, and no later label or arm is evaluated after a match.** Keeping $v$ on the evaluation [stack](../../../../../stack-data-structure.md) also preserves its original value if a label evaluation has a [side effect](../../../../../side-effect-computer-science.md) that changes a variable appearing in the controlling [program expression](../../../../../program-expression.md). A nested `Case` uses the same [stack invariant](../../../../../stack-invariant.md) relative to whatever [stack](../../../../../stack-data-structure.md) it receives. The concise contract is

$$
\boxed{N_{\mathrm{control}}=1,\quad N_{\mathrm{reached\ label}}=1,\quad \Delta h_{\mathrm{stack}}=0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
