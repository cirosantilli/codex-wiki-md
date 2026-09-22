<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here is a literal instruction selection for the trees in part (b), with the [temporary variables](../../../../../temporary-variable.md) allocated to [processor registers](../../../../../processor-register.md). `MOV r,#k` loads an arbitrary constant in one instruction. `LD` and `ST` load and store one four-[byte](../../../../../byte.md) word; `[r]` denotes zero-offset access. `LSL` is a [left shift](../../../../../left-shift.md). We use conventional base-plus-immediate access for the fixed local offset `I`.

```
MOV  rb, #A
LD   ri, [fp + I]
LSL  ru, ri, #2
ADD  ru, rb, ru
LD   rv, [ru]
LSL  rw, rv, #2
ADD  rw, rb, rw
LD   rt, [rw]
ST   rv, [rw]
ST   rt, [ru]
```

The first four instructions construct `u`, the fifth obtains `v`, the next two construct `w`, and the last three perform the remaining load and the two stores. Each destructive update of `ru` or `rw` reuses a [processor register](../../../../../processor-register.md) whose previous value is no longer needed. We assume enough [processor registers](../../../../../processor-register.md) to avoid a [register spill](../../../../../spilling-a-register.md).

If the target offers only the explicitly mentioned two-register [register-offset addressing](../../../../../register-offset-addressing.md) and lacks base-plus-immediate access, replace the one local load by `MOV rk,#I; LD ri,[fp+rk]`; all other conclusions are unchanged. A zero [processor register](../../../../../processor-register.md) or a zero-offset load supplies the notation `[ru]` and `[rw]` as usual. **This direct translation takes ten instructions with immediate local addressing, or eleven with the stated replacement.** Thus

$$
\boxed{N_{\mathrm{direct}}=10\quad\text{(11 with the register-only local load)}.}
$$

 These are instruction counts for the specified abstract target, not measured execution times.

## ↑ Ancestors (11)

1. [C](../c.md)
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
