<h1 id="c/2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Euler's totient function](../../../../../../euler-totient-function.md) $\phi(n)$ counts the [integers](../../../../../../integer-split.md) $1\le a\le n$ [coprime](../../../../../../coprime-integers.md) to $n$, equivalently the invertible [residue](../../../../../../residue.md) classes modulo $n$. Among $1,\ldots,p^e$, exactly the $p^{e-1}$ multiples of $p$ are not [coprime](../../../../../../coprime-integers.md) to the [prime power](../../../../../../prime-power.md). Hence

$$
\boxed{\phi(p^e)=p^e-p^{e-1}=p^e(1-1/p).}
$$

Factor $n=\prod_p p^{e_p}$. Its distinct prime-power factors are pairwise [coprime](../../../../../../coprime-integers.md), so the permitted [multiplicativity](../../../../../../multiplicativity-of-an-arithmetic-function.md) gives

$$
\phi(n)=\prod_{p\mid n}p^{e_p}(1-1/p)
=\boxed{n\prod_{p\mid n}(1-1/p).}
$$

For $n=1$, the [empty product](../../../../../../empty-product.md) is one and agrees with $\phi(1)=1$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [C](../../../../c.md)
5. [2005](../../../../../2005-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
