<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the Laurent generating function of the one-step [subdivision mask](../../../../../../subdivision-mask.md) as

$$
A(z,w)=\sum a_{ij}z^iw^j=\frac{(2+z+z^{-1})(2+w+w^{-1})}{8}=\frac{(1+z)^2(1+w)^2}{8zw}.
$$

For [quincunx subdivision](../../../../../../quincunx-subdivision.md), $p^{(1)}_j=\sum_i a_{j-Di}p_i$. A second step gives $p^{(2)}_k=\sum_{i,j}a_{k-Dj}a_{j-Di}p_i$. Setting $r=j-Di$ and $s=k-Dj$, its fine-grid offset is $k-2i=s+Dr$, since $D^2=2I$. Hence the binary mask is the convolution of $a$ with its $D$-transformed copy:

$$
\boxed{B(z,w)=A(z,w)A(zw,z/w)=\frac{(1+z)^2(1+w)^2(1+zw)^2(1+z/w)^2}{64z^3w}}.
$$

Expanding gives the centered binary propagation [subdivision mask](../../../../../../subdivision-mask.md), with row and column offsets running from $-3$ to $3$:

$$
\boxed{\frac1{64}\begin{pmatrix}
0&0&1&2&1&0&0\\
0&2&6&8&6&2&0\\
1&6&14&18&14&6&1\\
2&8&18&24&18&8&2\\
1&6&14&18&14&6&1\\
0&2&6&8&6&2&0\\
0&0&1&2&1&0&0
\end{pmatrix}}.
$$

The numerator entries sum to $256$, so $B(1,1)=4$, appropriate for a binary surface refinement. More specifically, each of the four parity classes sums to one after division by $64$, checking constant reproduction at every type of new lattice point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
