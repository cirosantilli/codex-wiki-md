<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The target's [register-offset addressing](../../../../../register-offset-addressing.md) already performs the [addition](../../../../../addition.md) of the array base and a scaled index as part of each load or store. Materializing a maximal common address expression into a [processor register](../../../../../processor-register.md) introduces an explicit `ADD` that this addressing mode could have supplied. Here the extra address [temporary variables](../../../../../temporary-variable.md) save no arithmetic that the memory instructions need to perform separately.

Instead keep the scaled indices, share the loaded old value of `a[i]`, and fold the base [addition](../../../../../addition.md) into each memory operand:

```
MOV  rb, #A
LD   ri, [fp + I]
LSL  rj, ri, #2
LD   rv, [rb + rj]
LSL  rk, rv, #2
LD   rt, [rb + rk]
ST   rv, [rb + rk]
ST   rt, [rb + rj]
```

`rj` remains the original index's byte offset, `rv` is its old element, and `rk` remains the second element's byte offset. Both stores use those saved offsets. **Folding address [additions](../../../../../addition.md) into the memory instructions removes two instructions, reducing ten to eight**, or eleven to nine if the local load requires the alternative sequence described in part (c). Therefore

$$
\boxed{N_{\mathrm{folded}}=N_{\mathrm{direct}}-2=8\quad\text{(or 9)}.}
$$

This illustrates why [common subexpression elimination](../../../../../common-subexpression-elimination.md) must interact with [instruction selection](../../../../../instruction-selection.md): a larger repeated tree is not automatically a better value to materialize. A useful refinement retains common scaled-index trees, or propagates the address [addition](../../../../../addition.md) trees back into their memory uses. The calculation establishes an instruction-count improvement under the stated [instruction set architecture](../../../../../instruction-set-architecture.md); scheduling and actual timing depend on further machine details.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
