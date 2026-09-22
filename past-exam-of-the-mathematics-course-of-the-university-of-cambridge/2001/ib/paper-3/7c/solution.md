<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

Call the four given column vectors $v_1,v_2,v_3,v_4$. Direct componentwise calculation gives

$$
v_3=2v_1+\frac12v_2,\qquad v_4=v_1+v_2.
$$

The first two vectors are independent: their first two components give the determinant $1\cdot2-4\cdot2=-6\ne0$. They form a [basis](../../../../../basis.md) of $W$, so $\boxed{\dim W=2}$.

Choose columns $v_1,v_2,0,0,-v_1-v_2$. This gives the [matrix](../../../../../matrix.md)

$$
\boxed{M=\begin{pmatrix}1&4&0&0&-5\\2&2&0&0&-4\\2&-2&0&0&0\\-1&6&0&0&-5\\1&-2&0&0&1\end{pmatrix}.}
$$

Its [image](../../../../../image-of-a-function.md) is exactly $W$, since all its columns belong to $W$ and its first two span $W$. Its column sum is zero, so $(1,1,1,1,1)^T$ belongs to its [kernel](../../../../../kernel-of-a-linear-map.md).

All [linear maps](../../../../../linear-map.md) with the stated kernel condition and image contained in $W$ factor uniquely through the [quotient vector space](../../../../../quotient-vector-space.md) $\mathbb R^5/\operatorname{span}\{(1,1,1,1,1)^T\}$. This quotient has dimension four. A [linear map](../../../../../linear-map.md) from it to the two-dimensional $W$ is specified by eight independent real coordinates, so the requested space has dimension $\boxed8$. Requiring the image to equal $W$, instead of being contained in $W$, would not define a vector space; the printed containment is essential.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
