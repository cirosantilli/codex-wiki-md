<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the conventional [integer](../../../../../integer-split.md) [calling convention](../../../../../calling-convention.md): `$a0` holds the argument and `$v0` holds the result. The function is recursive, so every call must preserve its own [return address](../../../../../return-address.md) and original argument. The first recursive result must also survive the second call; a [caller-saved register](../../../../../caller-saved-register.md) alone would not protect it.

This implementation reserves a 32-[byte](../../../../../byte.md) [stack frame](../../../../../stack-frame.md), keeping the [stack pointer](../../../../../stack-pointer.md) eight-[byte](../../../../../byte.md) aligned. Offsets 0–15 are available as the outgoing argument area, 16 stores the original argument, 20 stores the first result, 24 is padding, and 28 stores the [return address](../../../../../return-address.md). It changes no [callee-saved register](../../../../../callee-saved-register.md). Assemble in classic MIPS delayed-branch mode with instruction reordering disabled, such as `.set noreorder`.

```
foo:
addiu $sp,$sp,-32  # allocate 32-byte aligned frame
sw $ra,28($sp)  # save caller return address
sw $a0,16($sp)  # save original n
beq $a0,$zero,foo_base
sll $zero,$zero,0
addiu $t0,$zero,1
beq $a0,$t0,foo_base
sll $zero,$zero,0
addiu $t0,$zero,2
beq $a0,$t0,foo_base
sll $zero,$zero,0
addiu $a0,$a0,-1
jal foo
sll $zero,$zero,0
sw $v0,20($sp)  # preserve foo(n-1) across next call
lw $a0,16($sp)  # recover original n
sll $zero,$zero,0
addiu $a0,$a0,-3
jal foo
sll $zero,$zero,0
lw $t0,20($sp)
sll $zero,$zero,0
addu $v0,$v0,$t0  # combine the two recursive results
beq $zero,$zero,foo_return
sll $zero,$zero,0
foo_base:
addu $v0,$a0,$zero  # base case result is n
foo_return:
lw $ra,28($sp)
sll $zero,$zero,0
addiu $sp,$sp,32  # release the frame
jr $ra
sll $zero,$zero,0
```

All displayed operation mnemonics denote single [machine instructions](../../../../../machine-instruction.md). In particular, `sll $zero,$zero,0` is the actual harmless shift encoding often abbreviated by the [pseudoinstruction](../../../../../pseudoinstruction.md) `nop`; `addu $v0,$a0,$zero` performs a copy without the `move` [pseudoinstruction](../../../../../pseudoinstruction.md). Each branch or jump has an explicit harmless [branch delay slot](../../../../../branch-delay-slot.md), and harmless shifts also separate loads from their subsequent uses. The base cases return the original argument; other calls return the sum of the two recursive values. Every return restores the saved [return address](../../../../../return-address.md) and exactly undoes the stack allocation.[Revision 2.00, ADDIU and ADDU, pp. 37–38; JAL and JR, pp. 139 and 144](../../../../../mips32-architecture-for-programmers-volume-ii-by-mips-technologies.md)

The stated domain is [nonnegative integer](../../../../../natural-number.md) $n$, with sufficient stack space and a result representable in the intended [integer](../../../../../integer-split.md) type. The non-trapping additions implement that mathematical result within range; beyond it, machine wraparound would require a separately specified [integer](../../../../../integer-split.md) semantics.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
