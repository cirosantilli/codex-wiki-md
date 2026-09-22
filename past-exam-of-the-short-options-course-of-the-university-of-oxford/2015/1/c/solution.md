<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First simplify the specified residue by [modular exponentiation](../../../../modular-exponentiation.md). Modulo the [prime number](../../../../prime-number-split.md) $113$,

$$
102^2\equiv8,\quad102^4\equiv64,\quad102^8\equiv28,\quad
102^{16}\equiv106,\quad102^{32}\equiv49,\quad102^{64}\equiv28.
$$

Therefore $102^{70}\equiv28\cdot64\cdot8\equiv98$, so the required equation becomes $x^{37}\equiv97\pmod{113}$. Its right side is nonzero, so any solution is a [unit](../../../../unit-in-a-ring.md) modulo $113$.

By [Fermat's little theorem](../../../../fermat-little-theorem.md), exponents of such [units](../../../../unit-in-a-ring.md) can be reduced modulo $112$. Since

$$
37\cdot109=1+36\cdot112,
$$

raising to the $109$th power is the inverse of raising to the $37$th power. There is therefore exactly one residue class of solutions:

$$
x\equiv97^{109}\equiv97^{-3}\pmod{113}.
$$

Now $97\equiv-16$ and $97^3\equiv-4096\equiv85$. Since $4\cdot85\equiv1$, we obtain

$$
\boxed{x\equiv4\pmod{113}.}
$$

As a direct check, $4^4\equiv30$, $4^8\equiv109$, $4^{16}\equiv16$, and $4^{32}\equiv30$, whence $4^{37}\equiv30\cdot30\cdot4\equiv97$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
