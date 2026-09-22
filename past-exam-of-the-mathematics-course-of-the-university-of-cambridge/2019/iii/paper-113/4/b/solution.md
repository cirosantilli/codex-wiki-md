<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [cohomology of twisting sheaves on projective space](../../../../../../cohomology-of-twisting-sheaves-on-projective-space.md) is

$$
H^p(\mathbb P_k^r,\mathcal O(n))\cong
\begin{cases}
k[x_0,\ldots,x_r]_n,&p=0,\ n\geq0,\\
k[x_0,\ldots,x_r]_{-n-r-1}^{*},&p=r,\ n\leq-r-1,\\
0,&\text{otherwise}.
\end{cases}
$$

In particular, $H^i(X,\mathcal O_X)=H^i(X,\mathcal O_X(1))=0$ for $i>0$, while $H^0(X,\mathcal O_X)=k$ and $H^0(X,\mathcal O_X(1))\cong k^{r+1}$.

Apply the [long exact sequence in cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) to the displayed [Euler sequence](../../../../../../euler-sequence.md). Its degree-zero part is

$$
0\longrightarrow k\longrightarrow (k^{r+1})^{\oplus(r+1)}
\longrightarrow H^0(X,\mathcal T)\longrightarrow0,
$$

and all later terms vanish. The first map sends $1$ to the tuple of homogeneous coordinates and is injective. Therefore

$$
\boxed{H^i(X,\mathcal T)\cong
\begin{cases}
k^{(r+1)^2-1},&i=0,\\
0,&i>0.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
