<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Fix `sub` to mean $S,u,v\mapsto S,u-v$. If the depth-minimizing order evaluates the right operand $f$ before the left operand $e$, the [stack](../../../../../stack-data-structure.md) ends in $S,f,e$, so ordinary `sub` would compute the wrong sign. Two possible [instruction set architecture](../../../../../instruction-set-architecture.md) extensions are:

- Add `swap`, with $S,u,v\mapsto S,v,u$. After computing $f$ and then $e$, use `swap; sub` to obtain $e-f$. One general [zero-address instruction](../../../../../zero-address-instruction.md) handles every noncommutative binary operation and is useful elsewhere, but each reversed evaluation needs an extra instruction and extra execution time. It can be implemented without an additional operand [stack](../../../../../stack-data-structure.md) slot.
- Add reverse-operand variants, such as `rsub` with $S,u,v\mapsto S,v-u$, and analogously reverse division and other required operations. After computing $f$ and then $e$, a single `rsub` obtains $e-f$. This avoids the extra executed `swap`, but requires more opcodes and decoder support, usually one reverse form for each affected operation.

Both preserve the same peak operand [stack](../../../../../stack-data-structure.md) bound:

$$
\boxed{\text{deeper child first; use either operand swapping or a reverse-operand opcode.}}
$$

The first trades extra dynamic instructions for a smaller instruction set; the second trades a larger instruction set for fewer executed instructions. Neither extension makes order-sensitive [side effects](../../../../../side-effect-computer-science.md) safe to reorder.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
