<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $a$ be a root modulo $p^j$. Every lift to a residue modulo $p^{j+1}$ is uniquely $a+tp^j$ with $t\pmod p$. The [polynomial](../../../../../polynomial-split.md) expansion gives

$$
f(a+tp^j)\equiv f(a)+tp^jf'(a)\pmod{p^{j+1}}.
$$

Because $a\pmod p$ is a root and there are no common roots of $f$ and $f'$, $f'(a)$ is nonzero modulo $p$. Thus precisely one $t$ solves

$$
\frac{f(a)}{p^j}+t f'(a)\equiv0\pmod p.
$$

Every root at one level therefore has exactly one lift, and every root at the next level reduces to a root at the previous level. [Induction](../../../../../mathematical-induction.md) proves equality of the counts from $p$ to $p^l$. This is [simple-root Hensel lifting by successive residues](../../../../../simple-root-hensel-lifting-by-successive-residues.md) at finite precision; completeness is unnecessary for this finite-level assertion.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
