<h1 id="p/p1/solution">Solution</h1>

↑ **Parent:** [P1](../p1.md)

The first-column largest [pivot element](../../../../pivot-element.md) is four, so eliminate with multipliers $1/2,0,1/4$ below it. The augmented [matrix](../../../../matrix.md) becomes

$$
\begin{pmatrix}4&1&2&6&|&4\\0&1/2&2&-1&|&2\\0&2&4&4&|&4\\0&1&2&7/2&|&7/2\end{pmatrix}.
$$

[Partial pivoting](../../../../columnwise-partial-pivoting.md) in the second column swaps rows two and three because two is largest in modulus. The next elimination multipliers are $1/4$ and $1/2$. This gives

$$
\begin{pmatrix}4&1&2&6&|&4\\0&2&4&4&|&4\\0&0&1&-2&|&1\\0&0&0&3/2&|&3/2\end{pmatrix}.
$$

The third [pivot element](../../../../pivot-element.md) is already largest and the final multiplier below it is zero. [Back substitution](../../../../back-substitution.md) gives $z=1$, $y=3$, $x=-6$, $w=-1/2$. Therefore

$$
\boxed{(w,x,y,z)=(-1/2,-6,3,1).}
$$

The row swap must also reorder the previously stored first-column multipliers in $L$. The factors are

$$
\boxed{P=\begin{pmatrix}1&0&0&0\\0&0&1&0\\0&1&0&0\\0&0&0&1\end{pmatrix},\quad
L=\begin{pmatrix}1&0&0&0\\0&1&0&0\\1/2&1/4&1&0\\1/4&1/2&0&1\end{pmatrix},}
$$



$$
\boxed{U=\begin{pmatrix}4&1&2&6\\0&2&4&4\\0&0&1&-2\\0&0&0&3/2\end{pmatrix}.}
$$

Multiplying these factors verifies $PA=LU$. This is the required elimination with [partial pivoting](../../../../columnwise-partial-pivoting.md), not an alternative solution method.

## ↑ Ancestors (12)

1. [P1](../p1.md)
2. [P](../../p.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
