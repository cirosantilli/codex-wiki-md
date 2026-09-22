<h1 id="11i/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Iterate the [puncturing](../../../../../../../punctured-code.md) inequality from part (ii) $d-1$ times and then use part (i):

$$
A(n,d)
\le A(n-1,d-1)
\le\cdots\le A(n-d+1,1)
=2^{n-d+1}.
$$

This is the binary [Singleton bound](../../../../../../../singleton-bound.md):

$$
\boxed{A(n,d)\le2^{n-d+1}}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [11I](../../../11i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
