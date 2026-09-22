<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First form the [singleton set](../../../../../../singleton-mathematics.md) $\{b\}=F_1(b,b)$ and then use $F_2$ to take a [set union](../../../../../../set-union.md):

$$
U(a,b)=F_2\bigl(F_1(a,F_1(b,b)),a\bigr)=\bigcup\{a,\{b\}\}=a\cup\{b\}.
$$

The unused second argument of $F_2$ may be any term. Since $x\cap c=x\setminus(x\setminus c)$, a term using only the prescribed operation symbols is

$$
\boxed{G(a,b,c)=F_3\bigl(U(a,b),F_3(U(a,b),c)\bigr).}
$$

After substituting the displayed term for both occurrences of $U$, this is literally a term in $F_1,F_2,F_3$, and its value is $(a\cup\{b\})\cap c$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 128](../../../paper-128-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
