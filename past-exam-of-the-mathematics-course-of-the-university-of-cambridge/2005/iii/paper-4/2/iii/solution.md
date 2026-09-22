<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a [fundamental system of a root system](../../../../../../fundamental-system-of-a-root-system.md) $\{\alpha,\beta\}$. Distinct [simple roots](../../../../../../simple-root.md) have nonpositive inner product. Their [Cartan matrix](../../../../../../cartan-matrix.md) has diagonal entries two and off-diagonal entries $-p,-q$, where either $p=q=0$, or $p,q$ are positive integers. The [root-system finiteness lemma](../../../../../../root-system-finiteness-lemma.md) gives $pq<4$. After exchanging the simple roots, the possibilities are

$$
\begin{pmatrix}2&0\\0&2\end{pmatrix},\quad
\begin{pmatrix}2&-1\\-1&2\end{pmatrix},\quad
\begin{pmatrix}2&-1\\-2&2\end{pmatrix},\quad
\begin{pmatrix}2&-1\\-3&2\end{pmatrix}.
$$

Their angles and relative lengths determine the two simple roots up to an orthogonal transformation and common scaling, except that the two orthogonal components can be scaled separately.

To see that no extra roots remain unspecified, write a positive root $\gamma=m\alpha+n\beta$ with nonnegative integer coefficients. If it is not simple, some simple root $\delta$ has $(\gamma,\delta)>0$: otherwise $\|\gamma\|^2=m(\gamma,\alpha)+n(\gamma,\beta)\le0$. The [root reflection](../../../../../../root-reflection.md) in $\delta$ subtracts a positive integer multiple of $\delta$. The other coordinate stays nonnegative; since $\gamma$ is not proportional to $\delta$, it is positive, so the reflected root must still be positive by the defining sign property of a [fundamental system of a root system](../../../../../../fundamental-system-of-a-root-system.md). Its height decreases. Repeating reduces $\gamma$ to a simple root. Thus every root is in a [Weyl group](../../../../../../weyl-group.md) orbit of a simple root.

For the four matrices, applying their simple reflections gives, respectively, the following positive roots:

$$
\begin{array}{c|l}
A_1\oplus A_1&\alpha,\beta\\
A_2&\alpha,\beta,\alpha+\beta\\
B_2&\alpha,\beta,\alpha+\beta,\alpha+2\beta\\
G_2&\alpha,\beta,\alpha+\beta,\alpha+2\beta,\alpha+3\beta,2\alpha+3\beta
\end{array}
$$

where in the last two rows $\alpha$ is long, $\beta$ short. For example, $s_\beta(\alpha)=\alpha+q\beta$ and $s_\alpha(\beta)=\beta+\alpha$ for the displayed matrices when the convention is $a_{ij}=2(\alpha_i,\alpha_j)/(\alpha_i,\alpha_i)$. The sets comprising these positive roots and their negatives are invariant under both reflections, as direct substitution verifies. The height argument therefore shows they are the whole [root system](../../../../../../root-system.md). This proves the [classification of rank-two root systems](../../../../../../classification-of-rank-two-root-systems.md):

$$
\boxed{A_1\oplus A_1,\quad A_2,\quad B_2,\quad G_2.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
