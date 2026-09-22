<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $\chi$ be the quadratic character, equivalently the [Legendre symbol](../../../../../../legendre-symbol.md). Zero is included among the square [residue classes](../../../../../../residue-class.md). For every [integer](../../../../../../integer.md) $n$ its square-class indicator is

$$
1_{\{n\bmod q\text{ is a square}\}}=\frac{1+\chi(n)+1_{q\mid n}}2.
$$

For a nonzero [quadratic residue](../../../../../../quadratic-residue.md) the right side is one, for a nonresidue it is zero, and for a multiple of $q$ it is one. Summing over the interval, the character contribution is $O(\sqrt q\log q)$ by the previous part, while the number of multiples of $q$ is $N/q+O(1)$. Thus the required count is

$$
\boxed{\frac{N(q+1)}{2q}+O(\sqrt q\log q).}
$$

This counts the [integers](../../../../../../integer.md) in the interval whose [residue classes](../../../../../../residue-class.md) are squares. When the interval exceeds one period, repeated appearances are counted; the displayed main term could not describe a count of distinct [residue classes](../../../../../../residue-class.md) for arbitrary $N$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
