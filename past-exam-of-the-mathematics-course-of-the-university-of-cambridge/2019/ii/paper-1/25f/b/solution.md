<h1 id="25f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a $K$-basis $e_1,\ldots,e_n$ of $L$ and write

$$
\alpha=\sum_{i=1}^nx_ie_i,
$$

thereby identifying $L$ with $\mathbb A_K^n$. Let $M(x)$ be the $n\times n$ matrix whose $j$th column is the coordinate vector of $\alpha^{j-1}$ in this basis, for $1\leq j\leq n$.

Write the multiplication table as

$$
e_ie_j=\sum_{l=1}^nc_{ij}^{\,l}e_l
$$

with fixed [structure constants](../../../../../../structure-constant.md) $c_{ij}^{\,l}\in K$. Repeated multiplication shows that every entry of $M(x)$ is a polynomial in $x_1,\ldots,x_n$. Hence

$$
D(x)=\det M(x)\in K[x_1,\ldots,x_n].
$$

By the criterion supplied in the question,

$$
K[\alpha]=L
\quad\Longleftrightarrow\quad
1,\alpha,\ldots,\alpha^{n-1}\text{ are a basis}
\quad\Longleftrightarrow\quad
D(x)\ne0.
$$

Consequently

$$
\boxed{U=D(D)=\mathbb A_K^n\setminus V(D)},
$$

which is a [distinguished open set](../../../../../../distinguished-open-set.md), and therefore a [Zariski-open set](../../../../../../zariski-open-set.md). This is the determinant construction showing that [primitive elements form a principal Zariski-open set](../../../../../../primitive-elements-form-a-principal-zariski-open-set.md). No assertion that $D$ is nonzero is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25F](../../25f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
