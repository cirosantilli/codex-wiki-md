<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Cancel one unary symbol from each block at each round. Mark the first, middle and last delimiters by $L,C,E$, respectively; use $X$ for a cancelled symbol in the left block and $Y$ for one in the right block. These are extra tape symbols of the [Turing machine](../../../../../turing-machine.md), all distinct from $0,1$ and blank. No numerical counter is needed in the finite control.

Starting on the first zero, replace it by $L$, scan right through the first block of ones to replace the next zero by $C$, then scan right through the second block and replace its terminal zero by $E$. Move left to $C$. If the initial head is on a blank immediately before the first zero, first move right to that zero. The cancellation loop always starts with the head at $C$:

- Move right past the $Y$ symbols. If the next symbol is $E$, all right-hand ones have been cancelled; enter the successful cleanup below.
- Otherwise that symbol is $1$. Replace it by $Y$, move left past right-block symbols to $C$, and continue left past any $X$ symbols.
- If the next symbol is $1$, replace it by $X$. Move right past the $X$ symbols back to $C$ and repeat the loop.
- If instead the next symbol is $L$, the left block is exhausted while the right block still needed a cancellation. Enter the zero-result cleanup below.

After $k$ completed rounds, the invariant is

$$
L1^{m-k}X^kCY^k1^{n-k}E,\qquad0\leq k\leq\min\{m,n\}.
$$

It holds initially with $k=0$, and each completed round changes exactly one remaining $1$ in each block into the corresponding marker. This proves the cancellation count and preserves the locations of all delimiters.

For successful cleanup, the right block is entirely $Y$ symbols. From $C$, sweep right, erasing all $Y$ symbols and finally $E$, then move left across the erased blanks back to the still-present $C$. Erase $C$ and continue left, erasing each $X$, until reaching either the last surviving $1$ or $L$. Move one cell right and write the new terminal zero there. Move left through the surviving ones to $L$, replace $L$ by $0$, and halt. The remaining nonblank tape is exactly

$$
\boxed{01^{m-n}0\quad\text{if }m>n.}
$$

For example, $0111110110$ represents $m=5,n=2$ and becomes $01110$, representing three.

For zero-result cleanup, the head has reached $L$. Sweep right, erasing everything through $E$ while retaining $L$; after erasing $E$, move left across the blanks to $L$. Replace $L$ by $0$, write a second zero in the next cell, and halt. Thus if $m<n$ the machine returns $00$. If $m=n$, successful cleanup also leaves $00$. With this explicit choice of behaviour,

$$
\boxed{\text{the machine always halts and returns }01^{\max\{m-n,0\}}0.}
$$

Each sweep seeks a retained delimiter or an end marker a finite distance away. Each completed round removes one right-block $1$; after at most $n$ completed rounds either cleanup or left-block exhaustion occurs. The stated scans, writes and single-cell moves are implementable by finitely many states, so this is an implementation-level [Turing machine](../../../../../turing-machine.md) construction. The output $00$ represents zero; a negative integer cannot be represented in the unsigned [unary numeral system](../../../../../unary-numeral-system.md) specified here.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
