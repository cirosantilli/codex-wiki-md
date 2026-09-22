<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [strict diagonal dominance](../../../../../../strictly-diagonally-dominant-matrix.md) argument proves the estimate even on a nonuniform strictly increasing [spline knot sequence](../../../../../../spline-knot-sequence.md). Put $h_i=t_{i+1}-t_i>0$. Then $N_i$ has a rising piece of length $h_i$ and a falling piece of length $h_{i+1}$, while $M_i=2N_i/(h_i+h_{i+1})$. The same integrations as in part (b) give the [linear-spline mixed Gram matrix](../../../../../../linear-spline-mixed-gram-matrix.md)

$$
g_{ii}=\frac23,\qquad g_{i,i-1}=\frac{h_i}{3(h_i+h_{i+1})},\qquad
g_{i,i+1}=\frac{h_{i+1}}{3(h_i+h_{i+1})}.
$$

Only entries with indices in $1,\ldots,n$ are present. Thus $\sum_{j\ne i}|g_{ij}|\le1/3$ in every row.

For $Ga=b$, choose an index $i$ with $|a_i|=\|a\|_{\ell^\infty}$. The [reverse triangle inequality](../../../../../../reverse-triangle-inequality.md) then yields

$$
|b_i|\ge g_{ii}|a_i|-\sum_{j\ne i}|g_{ij}||a_j|
\ge\left(\frac23-\frac13\right)\|a\|_{\ell^\infty}.
$$

Hence $\|a\|_{\ell^\infty}\le3\|b\|_{\ell^\infty}$. Applying this to every $b$ proves

$$
\boxed{\|G^{-1}\|_{\ell^\infty}\le3,\qquad\|P_{\mathcal S}\|_\infty\le3\quad(k=2).}
$$

This is the [inverse infinity-norm bound from diagonal dominance](../../../../../../inverse-infinity-norm-bound-from-diagonal-dominance.md); no total positivity theorem is needed. The proof also gives invertibility directly by taking $b=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
