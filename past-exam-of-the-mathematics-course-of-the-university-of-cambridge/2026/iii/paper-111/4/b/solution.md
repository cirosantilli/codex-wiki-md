<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
a_{ij}=2\cos\left(\frac{\pi}{m_{ij}}\right),
\qquad c_i=x_1\cdots x_i,
\qquad c_0=1.
$$

In the [Geometric representation of a Coxeter group](../../../../../../geometric-representation-of-a-coxeter-group.md),

$$
\sigma(x_i)e_j=e_j+a_{ij}e_i,
$$

including $i=j$, since $a_{ii}=2\cos\pi=-2$. As $\beta_i=\sigma(c_{i-1})e_i$, telescoping gives

$$
\sigma(c_i)e_j-\sigma(c_{i-1})e_j
=a_{ij}\beta_i.
$$

Summing from $i=1$ to $j-1$ yields

$$
\beta_j=e_j+\sum_{i<j}a_{ij}\beta_i,
$$

or equivalently

$$
e_j=\beta_j-\sum_{i<j}2\cos\left(\frac{\pi}{m_{ij}}\right)\beta_i.
$$

Summing the same telescoping identity all the way to $n$ and substituting this first formula gives

$$
\begin{aligned}
\sigma(c)e_j
&=e_j+\sum_{i=1}^na_{ij}\beta_i\\
&=\beta_j+\sum_{i\geq j}2\cos\left(\frac{\pi}{m_{ij}}\right)\beta_i,
\end{aligned}
$$

which is the second required identity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
