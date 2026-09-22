<h1 id="c/c2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a nonzero [quadratic nonresidue](../../../../../../quadratic-nonresidue.md) $c\pmod q$. There is one because the squaring map on $\mathbb F_q^\times$ is two-to-one, so exactly half its elements are squares. The moduli $4,q,b$ are pairwise [coprime](../../../../../../coprime-integers.md), so the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) gives a positive [integer](../../../../../../integer-split.md) $k$ satisfying

$$
k\equiv1\pmod4,\qquad k\equiv c\pmod q,\qquad k\equiv1\pmod b.
$$

When $b=1$, the last condition is vacuous. In particular $k$ is odd and [coprime](../../../../../../coprime-integers.md) to $qb$. Since $k\equiv1\pmod4$, [Jacobi reciprocity](../../../../../../jacobi-reciprocity-law.md) gives

$$
\left(\frac qk\right)=\left(\frac kq\right)=-1,
\qquad
\left(\frac bk\right)=\left(\frac kb\right)=1,
\qquad
\left(\frac{-1}k\right)=1.
$$

As $t$ is odd, [multiplicativity of the Jacobi symbol](../../../../../../multiplicativity-of-the-jacobi-symbol.md) now yields

$$
\boxed{\left(\frac ak\right)=\left(\frac{\pm1}k\right)
\left(\frac qk\right)^t\left(\frac bk\right)=-1.}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [C2](../../../c2.md)
4. [C](../../../../c.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
