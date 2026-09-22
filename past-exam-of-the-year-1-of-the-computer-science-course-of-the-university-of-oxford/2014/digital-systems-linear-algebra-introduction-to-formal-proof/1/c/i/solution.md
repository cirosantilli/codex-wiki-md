<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use byte addresses, so adjacent 32-[bit](../../../../../../bit.md) [array](../../../../../../array-data-structure.md) elements are four bytes apart. The following [MIPS instructions](../../../../../../mips-instruction.md) include harmless `sll $zero,$zero,0` instructions in every [branch delay slot](../../../../../../branch-delay-slot.md); the second load is followed by another independent instruction before its value is consumed, also accommodating an early [MIPS architecture](../../../../../../mips-architecture.md) with a load-use delay. All mnemonics here denote individual [machine instructions](../../../../../../machine-instruction.md).

```
        beq   $t3,$zero,done  # n=0: do not access any array
        sll   $zero,$zero,0
loop:
        lw    $t4,0($t0)      # current a element
        lw    $t5,0($t1)      # current b element
        addiu $t0,$t0,4       # advance a; also separates lw from its use
        subu  $t6,$t4,$t5     # current difference, modulo 2^32
        sw    $t6,0($t2)      # store current c element
        addiu $t1,$t1,4
        addiu $t2,$t2,4
        addiu $t3,$t3,-1      # one fewer element remains
        bne   $t3,$zero,loop
        sll   $zero,$zero,0
done:
```

A [loop invariant](../../../../../../loop-invariant.md) at the head of the loop, after $k$ completed iterations, is that the three addresses point to elements $k$, the count is $n-k$, and every output element before $k$ equals the corresponding difference. One iteration reads element $k$, stores its difference and advances to $k+1$, preserving the [loop invariant](../../../../../../loop-invariant.md). The remaining count is a nonnegative [loop variant](../../../../../../loop-variant.md) decreasing by one, so the loop ends with $k=n$.

The code uses `subu` to avoid signed-overflow traps: the suffix does not restrict the operands to unsigned values. Its precise result is

$$
\boxed{c_i\equiv a_i-b_i\pmod{2^{32}}\quad(0\leq i<n).}
$$

For representable signed differences this is exactly $c_i=a_i-b_i$. If trapping signed arithmetic is required instead, use `sub` and assume all differences are representable. The [arrays](../../../../../../array-data-structure.md) must occupy valid word-aligned storage with no address wrap; the usual separate output [array](../../../../../../array-data-structure.md) avoids overwriting unread inputs.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
