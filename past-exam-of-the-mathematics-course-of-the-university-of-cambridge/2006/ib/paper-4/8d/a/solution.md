<h1 id="8d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The successive [divided differences](../../../../../../divided-difference.md) for nodes $-1,0,1,3$ are

$$
\begin{array}{c|r|r|r|r}
x&f[x]&f[x,x_{\rm next}]&f[x,x_{\rm next},x_{\rm next\ next}]&f[-1,0,1,3]\\\hline
-1&-7&4&-2&1\\
0&-3&0&2&\\
1&-3&6&&\\
3&9&&&
\end{array}
$$

Thus the [Newton interpolation polynomial](../../../../../../newton-polynomial.md) is

$$
\boxed{p(x)=-7+4(x+1)-2(x+1)x+(x+1)x(x-1).}
$$

Expanding the products gives the power form

$$
\boxed{p(x)=x^3-2x^2+x-3.}
$$

The four values verify the data. Uniqueness follows because the difference of two degree-at-most-three interpolants would have four distinct roots.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8D](../../8d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
