<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Continue the instruction convention above. The current [stack frame](../../../../../stack-frame.md) is now `s`'s. Its [static chain](../../../../../static-chain.md) passes through `r` to `p`; `q` is declared directly inside `p`, so the new `q` activation must receive a [static link](../../../../../static-link.md) to that same `p` [stack frame](../../../../../stack-frame.md). Let `T` be the offset of `p`'s parameter `t`.

Define `CALL q,1` to expect, above the pre-existing evaluation [stack](../../../../../stack-data-structure.md), the [static link](../../../../../static-link.md) for `q` followed by its one argument. It consumes these, creates `q`'s [stack frame](../../../../../stack-frame.md) with its [dynamic link](../../../../../dynamic-link.md) pointing to the current `s` activation, and leaves one return value when `q` returns. This explicit convention avoids dependence on a particular real [instruction set architecture](../../../../../instruction-set-architecture.md).

```
PUSHFP       ; s
LOAD SL      ; r
LOAD SL      ; p, the required static parent of q
DUP          ; preserve p for CALL while also using it to read t
LOAD T       ; replace the duplicate p address by p.t
CALL q,1     ; q(p.t), with static parent p and dynamic caller s
RETVAL       ; return q's result from s to r
```

Immediately before `CALL`, the evaluation [stack](../../../../../stack-data-structure.md) ends in `p-frame, 3`. **Two [static link](../../../../../static-link.md) traversals find both the argument's environment and the environment to pass to `q`.** In terms of the hidden argument and ordinary argument,

$$
\boxed{\mathrm{SL}_{q}=\mathrm{frame}_{p},\qquad y=t=3.}
$$

 An implementation that places the hidden [static link](../../../../../static-link.md) after the ordinary argument could use a different ordering of these same operations.

## ↑ Ancestors (11)

1. [C](../c.md)
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
