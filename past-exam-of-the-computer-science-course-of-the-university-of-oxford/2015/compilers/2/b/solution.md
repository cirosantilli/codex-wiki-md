<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We specify a small [stack machine](../../../../../stack-machine.md) instruction convention because the paper does not prescribe instruction spellings or numeric [stack frame](../../../../../stack-frame.md) offsets. `PUSHFP` pushes the current [frame pointer](../../../../../frame-pointer.md). `LOAD k` replaces a [stack](../../../../../stack-data-structure.md)-top frame address by the value at fixed offset `k` in that frame. Let `SL` be the [static link](../../../../../static-link.md) offset, `X` the offset of `p`'s `x`, and `Y` the offset of `q`'s parameter `y`. `ADD` pops two [integers](../../../../../integer-split.md) and pushes their sum. `RETVAL` returns the [stack](../../../../../stack-data-structure.md)-top value, removes the current activation and restores the caller through the usual [calling convention](../../../../../calling-convention.md).

```
PUSHFP       ; address of q's frame
LOAD SL      ; q's static link: address of p's frame
LOAD X       ; value of p.x
PUSHFP       ; address of q's frame, above x
LOAD Y       ; q's local parameter y
ADD          ; x + y
RETVAL       ; return the sum to s
```

One [static link](../../../../../static-link.md) traversal suffices for `x`, despite three intervening calls in the [dynamic chain](../../../../../dynamic-chain.md). `y` is local to `q`. In this execution the two loads produce $3$ and $3$, so the returned [integer](../../../../../integer-split.md) is $\boxed{6}$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
