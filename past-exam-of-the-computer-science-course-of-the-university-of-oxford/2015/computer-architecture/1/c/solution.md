<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Speculative execution](../../../../../speculative-execution.md) allows younger instructions to proceed while some condition on an older instruction is unresolved. Here the prediction is that a [store instruction](../../../../../store-instruction.md) will pass its [memory management unit](../../../../../memory-management-unit.md)'s protection and translation checks. Successful prediction avoids waiting; failure requires discarding younger work and taking the older instruction's [synchronous processor exception](../../../../../synchronous-processor-exception.md). A result computed speculatively must not become an irreversible architectural change before it is safe.

In the displayed five-stage [in-order pipeline](../../../../../in-order-pipeline.md), the [store instruction](../../../../../store-instruction.md)'s [memory address](../../../../../memory-address.md) is computed in EX and its memory operation is in MEM. Take the permission check to finish at the end of MEM, with a one-cycle [cache hit](../../../../../cache-hit.md), no [data hazards](../../../../../data-hazard.md) and sufficient [store buffer](../../../../../store-buffer.md) capacity. A concrete conservative implementation without [speculative execution](../../../../../speculative-execution.md) fetches no younger instruction until this check has passed. Compare the start of a stream of independent, nonfaulting [store instructions](../../../../../store-instruction.md):

| Instruction | Without speculation | With speculation |
| --- | --- | --- |
| First store | IF 1, ID 2, EX 3, MEM 4, WB 5 | IF 1, ID 2, EX 3, MEM 4, WB 5 |
| Second store | IF 5, ID 6, EX 7, MEM 8, WB 9 | IF 2, ID 3, EX 4, MEM 5, WB 6 |
| Third store | IF 9, ID 10, EX 11, MEM 12, WB 13 | IF 3, ID 4, EX 5, MEM 6, WB 7 |

The conservative version inserts three otherwise unnecessary cycles after each such [store instruction](../../../../../store-instruction.md), whereas the speculative version can start one instruction per cycle. For $N$ stores, counting through WB, the times are $4N+1$ and $N+4$ cycles. Thus

$$
\boxed{S_N=\frac{4N+1}{N+4}\longrightarrow4.}
$$

More generally, with a fraction $f$ of such [store instructions](../../../../../store-instruction.md) and no other delays, this particular interlock gives an asymptotic comparison $S=1+3f$. The maximum is four, not five: the permission check is resolved in MEM, so waiting for the empty store WB stage is unnecessary.

The baseline's interlock position matters. If it allows younger IF and ID work but prohibits younger EX until the end of the store's MEM stage, only one EX cycle is lost per store: successive stores reach EX in cycles $3,5,7,\ldots$, compared with $3,4,5,\ldots$ under [speculative execution](../../../../../speculative-execution.md), giving a limiting factor of two for that baseline. Holding at ID instead gives two lost cycles per store and a factor of three. **The fourfold figure compares against a pipeline that stops younger fetch; an implementation that already permits younger front-end work has a smaller remaining benefit.** The source specifies the five stages but does not prescribe this alternative's interlock position.[Question 1(c), printed p. 2, and Figure 1, printed p. 3](../../../../../computer-architecture-examination-paper-by-the-university-of-oxford-2015.md)

On a protection failure detected at the end of MEM, younger instructions occupy EX, ID and IF and can be invalidated before their normal WB. Younger [store instructions](../../../../../store-instruction.md) must also be prevented from draining from a [store buffer](../../../../../store-buffer.md) before validation. Earlier updates to [processor condition flags](../../../../../processor-condition-flag.md), if any, need delayed commitment or restoration too. This is what makes the prediction compatible with a [precise exception](../../../../../precise-exception.md); merely continuing to execute is insufficient.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
