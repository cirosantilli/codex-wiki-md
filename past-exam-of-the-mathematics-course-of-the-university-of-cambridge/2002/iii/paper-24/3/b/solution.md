<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Count affine solutions and then add the point at infinity. Over the [finite field](../../../../../../finite-field.md) $\mathbb F_2$, both values of $x$ give $x^3-x=0$, and both values of $y$ solve $y^2+y=0$. Hence there are four affine points. Over $\mathbb F_3$, all three values of $x$ give zero, and each has the two ordinates $0,2$, giving six affine points.

Over the [finite field](../../../../../../finite-field.md) $\mathbb F_{11}$, completing the square gives $(2y+1)^2=1+4(x^3-x)$. The square residues are $0,1,3,4,5,9$. For $x=0,1,\ldots,10$, the right sides and the corresponding numbers of ordinates are

$$
\begin{array}{c|rrrrrrrrrrr}
x&0&1&2&3&4&5&6&7&8&9&10\\\hline
1+4(x^3-x)\bmod11&1&1&3&9&10&8&5&3&4&10&1\\
\#\{y\}&2&2&2&2&0&0&2&2&2&0&2
\end{array}
$$

Their sum is sixteen. The resulting [elliptic-curve point counts over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) are

$$
\boxed{\#\widetilde E_2(\mathbb F_2)=5,\qquad\#\widetilde E_3(\mathbb F_3)=7,\qquad\#\widetilde E_{11}(\mathbb F_{11})=17.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
