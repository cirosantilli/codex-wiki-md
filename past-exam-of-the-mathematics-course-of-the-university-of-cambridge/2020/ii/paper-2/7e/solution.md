<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

The poles of $\csc^3z$ inside $|z|=4$ are $z=-\pi,0,\pi$. Near $z=k\pi$, write $z=k\pi+w$. Its [Laurent series](../../../../../laurent-series.md) begins

$$
\frac1{\sin^3z}
=(-1)^k\left(\frac1{w^3}+\frac1{2w}+O(w)\right),
$$

so the [residue](../../../../../residue.md) is $(-1)^k/2$. The sum of the three residues is

$$
-\frac12+\frac12-\frac12=-\frac12.
$$

The positively oriented [residue theorem](../../../../../residue-theorem.md) now gives

$$
\boxed{\int_C\frac{dz}{\sin^3z}
=2\pi i\left(-\frac12\right)=-\pi i}.
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
