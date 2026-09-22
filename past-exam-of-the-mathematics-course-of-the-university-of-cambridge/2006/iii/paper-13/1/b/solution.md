<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the reverse direction, rectangular discrepancy also controls pairings with arbitrary bounded real test functions. If $u:X\to[-1,1]$ and $v:Y\to[-1,1]$, decompose each into its positive and negative parts. For example, the [layer cake representation](../../../../../../layer-cake-representation.md) gives

$$
u_+(x)=\int_0^1 1_{\{u(x)>s\}}\,ds,\qquad u_-(x)=\int_0^1 1_{\{u(x)<-s\}}\,ds.
$$

Each of the four sign combinations in $u(x)v(y)$ is thus an integral of rectangular [indicator functions](../../../../../../indicator-function.md). The [triangle inequality](../../../../../../triangle-inequality.md) and the definition of the [cut norm](../../../../../../cut-norm.md) show that

$$
|\mathbb E_{x,y}f(x,y)u(x)v(y)|\leq4D(f).
$$

Now fix $x',y'$ and take $u(x)=f(x,y')$, $v(y)=f(x',y)$. The hypothesis $|f|\leq1$ makes these admissible tests. Multiplying their pairing by $f(x',y')$ and averaging gives

$$
0\leq Q(f)\leq\mathbb E_{x',y'}\left|\mathbb E_{x,y}f(x,y)f(x,y')f(x',y)\right|\leq4D(f).
$$

Consequently

$$
\boxed{Q(f)\leq4D(f),\qquad c_1=4c_2\text{ is admissible}.}
$$

Together with part (a), this proves [cut norm and rectangle fourth-moment equivalence](../../../../../../cut-norm-and-rectangle-fourth-moment-equivalence.md). The intended equivalence is quantitative smallness: along any family of bounded functions, the normalized rectangle fourth moments tend to zero if and only if the normalized [cut norms](../../../../../../cut-norm.md) tend to zero. It does not assert equality of the two constants or norms.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
