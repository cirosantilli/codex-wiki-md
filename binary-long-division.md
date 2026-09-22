# Binary long division

↑ **Parent:** [Long division](long-division.md)

For [integers](integer-split.md) $x\geq0$ and $y>0$, an [integer division](integer-division.md) [algorithm](algorithm-split.md) determines the [binary numeral system](binary-numeral-system.md) digits of a quotient by testing and conditionally subtracting successively halved multiples of the divisor. The [loop invariant](loop-invariant.md) $x=qy+r$, together with $0\leq r<y2^j$, makes each step a halving of the remaining quotient interval. Start with $q=0,r=x$ and $j$ large enough that $x<y2^j$. To decrease $j$ by one, subtract $y2^{j-1}$ from $r$ and add $2^{j-1}$ to $q$ exactly when $r\geq y2^{j-1}$. Both branches preserve the displayed equality and establish $0\leq r<y2^{j-1}$. When $j=0$, the [quotient](quotient.md) and [remainder](remainder.md) conditions hold.

## ↑ Ancestors (7)

1. [Long division](long-division.md)
2. [Euclidean division](euclidean-division.md)
3. [Integer](integer-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/6/c/solution.md)
