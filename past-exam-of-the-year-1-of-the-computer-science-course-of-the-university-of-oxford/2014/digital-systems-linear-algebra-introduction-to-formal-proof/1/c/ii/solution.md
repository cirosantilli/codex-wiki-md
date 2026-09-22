<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Make the code a leaf procedure called `array_diff`, copy the four argument [processor registers](../../../../../../processor-register.md) into the temporaries used above, and replace the final label by a return. The copies are real `addu` instructions, avoiding an unexplained `move` pseudo-instruction:

```
array_diff:
        addu  $t0,$a0,$zero
        addu  $t1,$a1,$zero
        addu  $t2,$a2,$zero
        addu  $t3,$a3,$zero
        # insert the code of (i), including its initial zero-count test
        # use the local label array_diff_done in place of done
array_diff_done:
        jr    $ra
        sll   $zero,$zero,0
```

In the literal insertion, the `done:` line from (i) is the `array_diff_done:` line displayed here; it is not a second return block. Under the usual [calling convention](../../../../../../calling-convention.md), temporary [processor registers](../../../../../../processor-register.md) are caller-saved. This procedure calls no other procedure and changes no saved [processor registers](../../../../../../processor-register.md), so it needs no [stack frame](../../../../../../stack-frame.md) or saved [return address](../../../../../../return-address.md).

For a 32-[bit](../../../../../../bit.md) constant $K$, define $H_K=\lfloor K/2^{16}\rfloor$ and $L_K=K\bmod2^{16}$ using its unsigned [binary representation](../../../../../../binary-number.md). Load it with `lui` followed by `ori`; both are single [MIPS instructions](../../../../../../mips-instruction.md). For base addresses $A,B,C$ and count $N$, the main program is:

```
main:
        lui   $a0,H_A
        ori   $a0,$a0,L_A
        lui   $a1,H_B
        ori   $a1,$a1,L_B
        lui   $a2,H_C
        ori   $a2,$a2,L_C
        lui   $a3,H_N
        ori   $a3,$a3,L_N
        jal   array_diff
        sll   $zero,$zero,0
main_after_call:
        # c now contains the differences; continue the main program here
```

Here each `H_...` and `L_...` is an assembler-time numeric constant, not an executed operation. `lui` places the high half and clears the low half; `ori` inserts the low half without [sign extension](../../../../../../sign-extension.md). Thus

$$
\boxed{(H_K\ll16)\mathbin{\mathrm{OR}}L_K=K.}
$$

The `jal` instruction saves the [return address](../../../../../../return-address.md) after its [branch delay slot](../../../../../../branch-delay-slot.md) in `$ra`; `jr $ra` resumes at `main_after_call`. A main routine that itself needs to return to a caller must save its incoming `$ra` before `jal` and restore it afterwards.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
