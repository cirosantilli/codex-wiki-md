<h1 id="8c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Adding the three equations for $s,t$ gives the necessary [solvability condition](../../../../../../solvability-condition.md) $a+b+c=3$. Conversely, subtraction of the first two and use of the third force

$$
s=\frac{a-b}{2},\qquad t=\frac{1-c}{2}.
$$

If $a+b+c=3$, these values also satisfy the first two equations: for example,

$$
1+s+t=\frac{3+a-b-c}{2}=a.
$$

The analogous calculation gives $1-s+t=b$. Thus existence and uniqueness hold exactly under the stated compatibility condition:

$$
\boxed{a+b+c=3,\qquad s=\frac{a-b}{2},\quad t=\frac{1-c}{2}.}
$$

For the three-variable system the [matrix](../../../../../../matrix.md) and data vector are

$$
A=\begin{pmatrix}5&2&-1\\2&5&-1\\-1&-1&8\end{pmatrix},
\qquad
\mathbf x=\begin{pmatrix}x\\y\\z\end{pmatrix},
\qquad
\mathbf b=\begin{pmatrix}1+s+t\\1-s+t\\1-2t\end{pmatrix},
\qquad A\mathbf x=\mathbf b.
$$

Perform [Gaussian elimination](../../../../../../gaussian-elimination.md) on the augmented matrix. The operations $R_2\leftarrow5R_2-2R_1$ and $R_3\leftarrow5R_3+R_1$ give

$$
\left[
\begin{array}{ccc|c}
5&2&-1&1+s+t\\
0&21&-3&3-7s+3t\\
0&-3&39&6+s-9t
\end{array}
\right].
$$

Each operation is an invertible row scaling followed by a row addition, so the solution set is preserved. Next $R_3\leftarrow7R_3+R_2$ gives

$$
\left[
\begin{array}{ccc|c}
5&2&-1&1+s+t\\
0&21&-3&3-7s+3t\\
0&0&270&45-60t
\end{array}
\right].
$$

Back substitution now yields

$$
z=\frac16-\frac{2t}{9},\qquad
y=\frac{3-7s+3t+3z}{21}
=\frac16-\frac s3+\frac t9,
$$

and then

$$
\boxed{x=\frac16+\frac s3+\frac t9,\qquad
y=\frac16-\frac s3+\frac t9,\qquad
z=\frac16-\frac{2t}{9}.}
$$

All three pivots are nonzero. Thus **the solution exists uniquely for every $s,t$**, the [matrix rank](../../../../../../matrix-rank.md) is $3$, and the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md) represented by $A$ is $\{\mathbf0\}$. The general [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) for a matrix with $m$ columns is

$$
\boxed{\operatorname{rank}A+\dim\ker A=m;}
$$

here $m=3$.

Finally, reverse the viewpoint and regard $x,y,z$ as prescribed. The necessary and sufficient condition already proved applies with $a=5x+2y-z$, $b=2x+5y-z$, $c=-x-y+8z$. Their sum is $6(x+y+z)$. Consequently $s,t$ can be recovered exactly when

$$
\boxed{x+y+z=\frac12.}
$$

When this holds, their unique values are $s=\tfrac32(x-y)$ and $t=\tfrac12(1+x+y-8z)$. **The allowable triples form an affine plane, not all of $\mathbb R^3$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8C](../../8c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
