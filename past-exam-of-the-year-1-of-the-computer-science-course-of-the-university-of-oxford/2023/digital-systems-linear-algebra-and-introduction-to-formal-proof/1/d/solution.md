<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $s=\mathbf1_{\{a<0\}}$, let $b=1023s$, and let $u=(a+b)\bmod1024$ denote the least nonnegative residue. Here $a$ is a signed 32-[bit](../../../../../bit.md) [two's complement](../../../../../two-s-complement.md) value. The source instructions, annotated with their derived values, are:
```
rem1024:
    asrs r3, r0, #31    // r3 = -s: all zero bits or all one bits
    lsrs r3, r3, #22    // r3 = b = 1023*s
    adds r0, r0, r3     // r0 = a+b
    lsls r0, r0, #22    // r0 has word value (a+b)*2^22 modulo 2^32
    lsrs r0, r0, #22    // r0 = u = (a+b) modulo 1024, in 0,...,1023
    subs r0, r0, r3     // r0 = u-b
    bx lr              // return u-b
```
The first instruction is an [arithmetic right shift](../../../../../arithmetic-right-shift.md), so it replicates the sign [bit](../../../../../bit.md). The second is a [logical right shift](../../../../../logical-right-shift.md), turning the all-one word into $1023$. The paired shifts then extract the low ten [bits](../../../../../bit.md), as in (c). Their effect is the residue of $a+b$ even if its [two's complement](../../../../../two-s-complement.md) interpretation is negative, because $1024$ divides the word modulus $2^{32}$. The adjusted value $a+b$ is representable for every input: positive inputs are unchanged, and negative inputs gain only $1023$.

For $a\geq0$, $b=0$, so the return value is the usual nonnegative remainder $a\bmod1024$. For $a<0$, put $t=-a>0$ as a mathematical [integer](../../../../../integer-split.md), and write $t=1024q+r$ with $0\leq r<1024$. If $r=0$, then $u=1023$ and the return value is zero. If $1\leq r\leq1023$, then

$$
u=(-t+1023)\bmod1024=1023-r,
\qquad u-b=-r.
$$

These are precisely the remainders for [C integer division](../../../../../c-integer-division.md), whose quotient truncates towards zero. In every case the result has the dividend's sign or is zero, has magnitude below $1024$, and satisfies $a=1024q_C+r_C$. The proof includes the smallest representable input: $t=-a$ was used only in mathematical reasoning, not as an overflowing machine operation.[section 6.5.5 paragraph 6, quotient truncation and the quotient–remainder identity](../../../../../c11-committee-draft-n1570.md)

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
