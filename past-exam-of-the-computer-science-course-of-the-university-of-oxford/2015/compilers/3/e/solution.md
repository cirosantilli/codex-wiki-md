<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The source rewrite already saves the old `a[i]` in register-allocated `t`. Denote the original [integer](../../../../../integer-split.md) index by $i_0$, its original element by $j=a[i_0]$, and the original element there by $k=a[j]$. The second fragment first sets `t=j`, then writes $k$ to `a[i0]`, and finally writes $j$ to `a[j]`. Thus it performs the same intended swap without needing to recompute the second [memory address](../../../../../memory-address.md) from a possibly modified array element.

For completeness, the first fragment is also correct when the two locations might alias. If $j\ne i_0$, its middle store changes only `a[j]`, so the final `a[i]` still denotes the first location. If $j=i_0$, then $k=a[j]=a[i_0]=j=i_0$, and the supposed swap is a no-op in both fragments. There is no need to assume distinct locations.

For the second fragment, [common subexpression elimination](../../../../../common-subexpression-elimination.md) of maximal addresses gives, using `z` for the second address:

```
MOVE(R(u), ADD(C(A),SHL(M(ADD(R(fp),C(I))),2)))
MOVE(R(t), M(R(u)))
MOVE(R(z), ADD(C(A),SHL(R(t),2)))
MOVE(M(R(u)), M(R(z)))
MOVE(M(R(z)), R(t))
```

The nested memory-to-memory assignment requires an additional scratch [processor register](../../../../../processor-register.md) `rv` on a [reduced instruction set computer](../../../../../reduced-instruction-set-computer.md). A direct translation is therefore:

```
MOV  rb, #A
LD   ri, [fp + I]
LSL  ru, ri, #2
ADD  ru, rb, ru
LD   rt, [ru]
LSL  rz, rt, #2
ADD  rz, rb, rz
LD   rv, [rz]
ST   rv, [ru]
ST   rt, [rz]
```

**The same compiler need not produce any better code: this has the same ten-instruction count as part (c).** It still performs two element loads, two element stores, two shifts and two separately materialized address additions, plus the base and local-index setup. The [processor register](../../../../../processor-register.md) roles and store order differ, but the work is the same. The corresponding folding of [register-offset addressing](../../../../../register-offset-addressing.md) removes both `ADD` instructions here too, yielding the same eight-instruction count as part (d).

The key [alias analysis](../../../../../alias-analysis.md) advantage available in both fragments is that `i` remains unchanged by the array stores. In the second fragment, `t` is also unchanged after its first assignment because it lives in a [processor register](../../../../../processor-register.md). Its name alone does not produce a further saving beyond what the first fragment's [common subexpression elimination](../../../../../common-subexpression-elimination.md) already achieves. Exact [instruction selection](../../../../../instruction-selection.md) is not uniquely prescribed by the paper; these explicit translations demonstrate why the claimed source-level efficiency advantage does not follow:

$$
\boxed{N_{\mathrm{second}}=N_{\mathrm{first}}=10\quad\text{(both reduce to 8 after address folding)}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
