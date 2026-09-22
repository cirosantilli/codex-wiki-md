<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

The line through the origin is $l_0=\operatorname{span}(u)$, containing zero and closed under addition and scalar multiplication, so it is a [vector subspace](../../../../../vector-subspace.md). If $l_{x_1}=l_{x_2}$, then $x_1\in l_{x_2}$ and $x_1=x_2+\lambda u$ for some real $\lambda$. Conversely that equality gives the same set after shifting the line parameter. Thus

$$
\boxed{l_{x_1}=l_{x_2}\iff x_1-x_2\in\operatorname{span}(u).}
$$

Changing representatives to $x'=x+su$, $y'=y+tu$ changes their sum by $(s+t)u$ and a scalar multiple by $\alpha su$. The line classes therefore do not change, proving both operations well-defined. Associativity follows from $l_{(x+y)+z}=l_{x+(y+z)}$. The zero vector of this [quotient vector space](../../../../../quotient-vector-space.md) is **the entire line $l_0$**, because $l_x+l_0=l_x$.

For a [basis](../../../../../basis.md) $(u,b_1,b_2)$ of $\mathbb R^3$, every vector is $x=su+tb_1+vb_2$, so $l_x=t l_{b_1}+v l_{b_2}$. If this combination equals $l_0$, then $tb_1+vb_2=su$; independence of the three original [basis vectors](../../../../../basis-vector.md) forces $t=v=s=0$. Hence **$(l_{b_1},l_{b_2})$ is a basis** of the space of [parallel lines as a quotient vector space](../../../../../parallel-lines-as-a-quotient-vector-space.md).

For the specified direction, add $zu$ to $(x,y,z)^T$ to obtain the representative $(x+z,y+3z,0)^T$. Thus its coordinates in the two standard line classes are $(x+z,y+3z)^T$. The two supplied image classes have coordinates $(1,1)^T$ and $(-3,1)^T$, while their input coordinates are $(1,-1)^T$ and $(1,1)^T$. If $a_1,a_2$ are the matrix columns, then $a_1-a_2=(1,1)^T$ and $a_1+a_2=(-3,1)^T$. Solving gives

$$
\boxed{A=\begin{pmatrix}-1&-2\\1&0\end{pmatrix}.}
$$

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
